<script>
    import "../app.css";
    import Nav from "../components/Nav.svelte";
</script>
<div class="flex justify-center items-center h-screen">
    <div class="grid sm:grid-cols-[auto,1fr] gap-4 m-auto w-max">
            <img class=" max-w-[89px] sm:justify-self-end" src="me.png" alt="headshot of me">
            <div class="self-end">
                <h1 class="text-3xl font-bold">Chase Almy</h1>
                <h4>Process Focused UI Developer</h4>
            </div>
            <Nav/>
        <slot />
    </div>

</div>
