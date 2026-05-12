<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /><title>Louis Abery Portfolio</title></svelte:head>

<nav class="p-6 border-b border-black gap-6 items-center">
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

{@render children()}

<footer class="flex items-center justify-center p-4">
    <p>&copy; 2026 Louis Abery</p>
</footer>