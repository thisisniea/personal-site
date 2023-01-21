<script lang="ts">
  import Nav from "./lib/Nav.svelte";

  import Spotlight from "./lib/Spotlight.svelte";

  const age = Math.floor((new Date().getTime() - new Date("2003-08-07").getTime()) / 1000 / 60 / 60 / 24 / 365);
</script>

<Nav />

<main>
  <h1>
    Creative technologist,<br />
    low-level software developer<abbr title="Oxford comma">,</abbr><br />
    and cat enthusiast.
  </h1>

  <p>
    Hi, my name is Brandon, and I'm a {age}-year-old hobbyist developer from The
    United States. I'm passionate about exploring the low-level world, ranging from
    reverse engineering to assembly language programming, operating systems tinkering,
    and more. Crafting web applications from scratch is another joy of mine and
    the one that inspired me to create this site!
  </p>

  <p>
    Please take a look at some of my amazing projects in the Spotlight section below.
    You can also connect with me on some of the social media sites that I have an account on.
    I appreciate your visit to my site and thank you for taking the time to check it out!
  </p>

  <hr />

  <Spotlight />
</main>

<style lang="postcss">
  main {
    padding: 5rem 1rem 1rem 1rem;
    max-width: 800px;
    margin: 0 auto;
  }

  abbr {
    text-decoration: none;
  }

  h1 {
    font-size: 2.5rem;
    margin: 0;
    padding: 0;
    margin-bottom: 2rem;
    margin-left: -1rem;
    width: calc(100% + 2rem);
  }

  @media (max-width: 900px) {
    br {
      display: none;
    }

    h1 {
      margin-left: 0;
      width: fit-content;
    }
  }
</style>
