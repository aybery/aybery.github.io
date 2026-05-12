<script>
    import { page } from '$app/state';
    import { resolve } from '$app/paths';
</script>

<div class="flex flex-col items-center justify-center p-4">   
    <h1>Error <span class="text-red-600">{page.status}</span></h1>
    <p class="font-bold">{page.error?.message || 'Page not found'}</p>
    <a href={resolve('/')} class=" font-extrabold text-blue-500 hover:underline">← Go Home</a>
</div>