<script lang="ts">
  import { onMount } from 'svelte';
  import { user, signOut } from '@/lib/auth';
  import { startHealthPolling, type HealthStatus } from '@/lib/health';

  let apiStatus: HealthStatus = $state('checking');

  onMount(() => startHealthPolling((status) => {
    apiStatus = status;
  }));

  const statusLabel = $derived(
    apiStatus === 'checking'
      ? 'Checking API…'
      : apiStatus === 'online'
        ? 'API online'
        : 'API offline',
  );

  const statusColor = $derived(
    apiStatus === 'checking'
      ? 'bg-amber-400'
      : apiStatus === 'online'
        ? 'bg-green-500'
        : 'bg-red-500',
  );
</script>

<header class="sticky top-0 z-50 border-b border-slate-200 bg-white/95 backdrop-blur">
  <div class="mx-auto flex h-14 max-w-5xl items-center justify-between gap-4 px-4">
    <div class="flex items-center gap-3">
      <div
        class="flex h-8 w-8 items-center justify-center rounded-md bg-slate-900 text-xs font-bold text-white"
        aria-hidden="true"
      >
        SA
      </div>
      <span class="font-semibold text-slate-900">Svelte Supabase Auth</span>
    </div>

    <div class="flex items-center gap-3">
      <div
        class="flex items-center gap-2 text-sm text-slate-500"
        title={statusLabel}
      >
        <span class={`h-2.5 w-2.5 rounded-full ${statusColor}`}></span>
        <span class="hidden sm:inline">{statusLabel}</span>
      </div>

      {#if $user}
        <span class="hidden text-sm text-slate-500 md:inline">{$user.email}</span>
        <button
          type="button"
          class="rounded-md border border-slate-300 bg-white px-3 py-1.5 text-sm font-medium text-slate-700 hover:bg-slate-50"
          onclick={() => signOut()}
        >
          Sign out
        </button>
      {/if}
    </div>
  </div>
</header>
