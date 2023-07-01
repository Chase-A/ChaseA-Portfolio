<script>
  import { page } from '$app/stores';
  let links = ['projects', 'experience', 'about']

  function toCapitalCase(str) {
    return str.toLowerCase().replace(/(^|\s)\w/g, function(match) {
      return match.toUpperCase();
    });
  }
</script>

<nav class="flex sm:flex-col gap-4 sm:gap-0 col-span-2 sm:col-span-1 sm:justify-self-end sm:justify-start sm:items-end">
    {#each links as link}
        <a class="w-max text-right hover:underline {('/'+ link) === $page.url.pathname ? 'underline': ''}" href="/{link}">{toCapitalCase(link)}</a>
    {/each}
</nav>