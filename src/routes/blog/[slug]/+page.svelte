<script lang="ts">
  import '$lib/styles/rehype.css'
  import type { PageData } from './$types'
  export let data: PageData
  const { title, date, description, categories, Content } = data
</script>

<svelte:head>
  <title>gubasso.xyz - Blog - {title}</title>
  <meta property="og:title" content={title} />
</svelte:head>

<article>
  <!-- <h1>{data.title}</h1> -->
  <!-- <p>Published: {data.date}</p> -->
  <!-- <svelte:component this={data.content} /> -->
  <h1>{title}</h1>
  <h2>Description: {description}</h2>
  <p>Published: {date}</p>
  {#if categories?.length}
    <p>Categories:</p>
    <ul>
      {#each categories || [] as cat}
        <li>
          <a href="/blog/categories/{cat}">{cat}</a>
        </li>
      {/each}
    </ul>
  {/if}
  <Content />
</article>
