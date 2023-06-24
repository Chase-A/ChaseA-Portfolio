<script>
    import "../app.css";
</script>
<div class="flex justify-center items-center h-screen">
    <div class="grid sm:grid-cols-[auto,1fr] gap-4 m-auto w-max">
            <img class=" max-w-[89px] sm:justify-self-end" src="me.png" alt="headshot of me">
            <div class="self-end">
                <h1 class="text-3xl font-bold">Chase Almy</h1>
                <h4>Process Focused UI Developer</h4>
            </div>
        
        <nav class="flex sm:flex-col justify-between sm:justify-self-end">
            <a href="/about" class=" text-right">About</a>
            <a href="/experience" class=" text-right">Experience</a>
            <a href="/projects" class=" text-right">Projects</a>
        </nav>
        
        <slot />
    </div>

</div>
