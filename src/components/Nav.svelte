<script>

import { page } from '$app/stores';

let links = ['about', 'experience', 'projects']

function toCapitalCase(str) {
  return str.toLowerCase().replace(/(^|\s)\w/g, function(match) {
    return match.toUpperCase();
  });
}

</script>





<nav class="flex sm:flex-col justify-between sm:justify-self-end">
    {#each links as link}
        <a class="text-right hover:underline {('/'+ link) === $page.url.pathname ? 'underline': ''}" href="/{link}">{toCapitalCase(link)}</a>
    {/each}
</nav>