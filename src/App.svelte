<script lang="ts">
  import Nav from './lib/Nav.svelte'

  import Home from './pages/Home.svelte'
  import About from './pages/About.svelte'
  import Projects from './pages/Projects.svelte'
  import Tools from './pages/Tools.svelte'

  let activeNum: number = 0
</script>

<Nav bind:activeNum={activeNum} />

<main>
  {#if activeNum === 0}
    <Home />
  {:else if activeNum === 1}
    <About />
  {:else if activeNum === 2}
    <Projects />
  {:else if activeNum === 3}
    <Tools />
  {/if}
</main>

<style lang="postcss">
  main {
    padding: 4rem 1rem 1rem 1rem;
    max-width: 800px;
    margin: 0 auto;
  }

  @media (min-width: 600px) {
    main {
      padding: 6rem 1rem 1rem 1rem;
    }
  }

  @media (min-width: 800px) {
    main {
      padding: 8rem 2rem 1rem 2rem;
    }
  }

</style>