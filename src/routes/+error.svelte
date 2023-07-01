<script>
    import { goto } from '$app/navigation';
    import { onMount } from 'svelte';
        onMount(() => {
        goto('projects');
    });
    
</script>


<main>
    <h1>404 Page Not Found</h1>
    <p>Oops! The page you are looking for does not exist.</p>
</main>