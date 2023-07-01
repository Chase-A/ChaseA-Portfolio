<script>
    import ProjectEntry from "$lib/components/ProjectEntry.svelte";
    import projects from "$lib/data/projects.json"
</script>

<section class="col-span-2 sm:col-span-1">
    {#each projects as project}
        <ProjectEntry {...project}/>
    {/each}
</section>