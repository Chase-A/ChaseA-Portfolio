<script>
    import WorkEntry from '$lib/components/Workentry.svelte'
    import workEntries from '$lib/data/work.json'
    import "../../app.css";
</script>

<section class="flex justify-center items-center h-screen">
    <div class="m-auto w-max max-w-[600px] mt-6">
        <div class="flex mb-6">
            <img class="max-w-[89px] justify-self-end" src="me.png" alt="headshot of me">
            <div class="self-end ml-6">
                <h1 class="text-5xl font-bold">Chase Almy</h1>
                <p class="text-gray-500">Process Focused UI Developer</p>
            </div>
        </div>
        {#each workEntries as entry}
            <WorkEntry {...entry}/>
        {/each}
        <div class="mb-6">
            <h2 class="text-2xl font-bold">Education</h2>
            <p>The Internet - 2004-Present</p>
            <p>Boston University - 2019-2022</p>
        </div>
        <div class="flex">
            <a class="mr-12 font-bold text-2xl self-center hover:underline" href="portfolio.com" >Portfolio:</a>
            <img class=" max-w-[140px]" src="/portfolio.png" alt="qr code linking to my portfolio">
        </div>
    </div>

</section>