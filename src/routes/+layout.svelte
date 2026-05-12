<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { resolve } from '$app/paths';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /><title>Louis Abery Portfolio</title></svelte:head>

<nav class="p-6 flex gap-6 items-center border-b border-black">
    <a href={resolve('/#home')}>Home</a>
    <a href={resolve('/#projects')}>Projects</a>
    <a href={resolve('/#contact')}>Contact</a>
</nav>

{@render children()}

<footer class="flex items-center justify-center p-4">
    <p>&copy; 2026 Louis Abery.</p>
</footer>