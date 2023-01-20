<script lang="ts">
  import Nav from './lib/Nav.svelte'

  import Home from './pages/Home.svelte'
  import Projects from './pages/Projects.svelte'
  import Tools from './pages/Tools.svelte'

  let activeNum: number = 0
</script>

<Nav bind:activeNum={activeNum} />

<main>
  {#if activeNum === 0}
    <Home />
  {:else if activeNum === 1}
    <Projects />
  {:else if activeNum === 2}
    <Tools />
  {/if}
</main>

<style lang="postcss">
  main {
    padding: 5rem 1rem 1rem 1rem;
    max-width: 800px;
    margin: 0 auto;
  }
</style>