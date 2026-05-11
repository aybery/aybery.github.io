<script>
    import { page } from '$app/state';
</script>

<h1>Oops! {page.status}</h1>
<p>{page.error?.message || 'Page not found'}</p>
