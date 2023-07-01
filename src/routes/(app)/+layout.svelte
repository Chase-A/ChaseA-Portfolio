<script>
    import "../../app.css";
    import Nav from "$lib/components/Nav.svelte";
    import { page } from '$app/stores';
    const title = $page.url.searchParams.get('t');
</script>
<div class="flex justify-center items-center h-screen p-4">
    <div class="grid grid-cols-[1fr,7fr] sm:grid-cols-[auto,1fr] gap-6 sm:gap-6 m-auto w-max max-w-lg sm:mt-24">
            <img class="max-w-[89px] sm:justify-self-end" src="me.png" alt="headshot of me">
            <div class="self-end">
                <h1 class="text-4xl sm:text-5xl font-bold">Chase Almy</h1>
                <p class="text-gray-500 text-sm sm:text-base">{title ? title : 'Process Focused UI Developer'}</p>
            </div>
            <Nav/>
        <slot class=""/>
    </div>
</div>

<style>
    /* :global(a) {
        position: relative;
    }

    :global(a::after) {
        content: "";
        position: absolute;
        bottom: 0;
        left: 0;
        width: 16px;
        height: 1px;
        background-color: var(--primary-color);
    } */
</style>