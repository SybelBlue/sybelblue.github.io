<script lang="ts">
	import type { Snippet } from 'svelte';
	import '../app.css';

	let { children }: { children?: Snippet<[]> } = $props();
</script>
<header>
  header
</header>
<main>
	{@render children?.()}
</main>

<style lang="postcss">
  header {
    @apply border-2 h-2;
  }
  main {
    @apply absolute overflow-hidden size-full bg-base-100;
  }
</style>