<script lang="ts">
  import type { PageData } from './$types'
  export let data: PageData
  let { categories } = data
</script>

<svelte:head>
  <title>gubasso.xyz - Blog - All Categories</title>
</svelte:head>

{#if categories.length}
  <h1>All categories:</h1>
  <ul>
    {#each categories as cat}
      <li>{cat}</li>
    {/each}
  </ul>
{:else}
  <h1>No category is registered</h1>
{/if}
