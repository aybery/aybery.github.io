<script>
    import { page } from '$app/state';
    import { resolve } from '$app/paths';
</script>

<h1>Oops! {page.status}</h1>
<p>{page.error?.message || 'Page not found'}</p>
<a href={resolve('/')}>Go Home</a>
