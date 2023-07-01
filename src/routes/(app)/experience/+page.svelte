
<script>
    import WorkEntry from '$lib/components/Workentry.svelte'
    import workEntries from '$lib/data/work.json'
</script>

<section class="col-span-2 sm:col-span-1">
    {#each workEntries as entry}
        <WorkEntry {...entry}/>
    {/each}
    <div class="mb-6">
        <h2 class="text-2xl font-bold">Education</h2>
        <p>The Internet - 2004-Present</p>
        <p>Boston University - 2019-2022</p>
    </div>

</section>



