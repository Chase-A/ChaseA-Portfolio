<script>
    export let img_url;
    export let title;
    export let employer;
    export let startDate;
    export let endDate;
    export let responsibilities;
</script>

<div class="mb-6">
    <div class="flex mb-2 items-center">
        <img class=" max-w-[40px] block object-contain" src="{img_url}" alt="{employer} logo">
        <div class=" ml-3">
            <h3 class="text-2xl font-bold leading-6">{title}</h3>
            <p class="text-gray-500 text-sm">{employer} - {startDate}{endDate === startDate ? '': '-'}{endDate ? (endDate === startDate ? '': endDate): 'Present'}</p>
        </div>
    </div>
    <ul>
        {#each responsibilities as responsibility}
            <li>{responsibility}</li>
        {/each}
    </ul>
</div>