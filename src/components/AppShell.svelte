<script lang="ts">
  import type { Snippet } from 'svelte';
  import AppHeader from '@/components/AppHeader.svelte';

  let { children }: { children: Snippet } = $props();
</script>

<div class="flex min-h-screen flex-col bg-slate-50">
  <AppHeader />
  <main class="mx-auto w-full max-w-5xl flex-1 p-4">
    {@render children()}
  </main>
</div>
