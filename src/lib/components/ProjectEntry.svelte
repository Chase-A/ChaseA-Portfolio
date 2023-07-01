<script>
    export let title
    export let description
    export let links
</script>

<div class="mb-6">
    <h3 class="text-2xl font-bold mb-2">{title}</h3>
    <p class="mb-2">{description}</p>
    <div class="flex flex-wrap gap-x-4 gap-y-2">
        {#each links as link}
            <a class="hover:underline" href="{link.url}" target="_blank" rel="noopener noreferrer">{link.name}</a>
        {/each}
    </div>
</div>