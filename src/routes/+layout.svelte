<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { resolve } from '$app/paths';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /><title>Louis Abery Portfolio</title></svelte:head>

<nav class="p-6 flex gap-6 items-center justify-center border-b border-gray-300 sticky top-0 z-50 bg-gray-950 font-bold text-2xl">
    <a href={resolve('/')} class="hover:text-blue-500 ease-in-out duration-300">Home</a>
    <a href={resolve('/#projects')} class="hover:text-blue-500 ease-in-out duration-300">Projects</a>
    <a href={resolve('/#contact')} class="hover:text-blue-500 ease-in-out duration-300">Contact</a>
</nav>

{@render children()}

<footer class="flex items-center justify-center p-4">
    <p>&copy; 2026 Louis Abery.</p>
</footer>