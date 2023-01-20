<script lang="ts">
    import Socials from "../lib/Socials.svelte";
import Spotlight from "../lib/Spotlight.svelte";

    // calculate age
    const age = Math.floor((new Date().getTime() - new Date("2003-08-04").getTime()) / 1000 / 60 / 60 / 24 / 365);

</script>

<h1>
    Creative technologist, <br>
    low-level software developer<abbr title="Oxford comma">,</abbr> <br>
    and cat enthusiast.
</h1>

<p class="para">
    Hi, my name is Brandon, and I'm a {age}-year-old hobbyist developer from The United States.
    I have a strong pulse and genuine interest in all things low-level, including reverse engineering, assembly language
    programming, and operating systems tinkering. Besides that, I also take great pleasure in developing web applications
    from scratch - which is why this website was born!
</p>

<p class="para">
    Here you will find a comprehensive directory of all my projects, so you can easily explore the
    work that I have done. Furthermore, you can get to know me better by reading through my personal profile. Finally,
    if you're curious about my activity on social media platforms such as Twitter and YouTube, then you'll be able
    to stalk me there too!
</p>

<Socials />

<hr>

<Spotlight />

<style lang="postcss">
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

    /* ripply line like a sine wave, but with a bit lower frequency */
    hr {
        border: none;
        border-bottom: 1px solid rgba(var(--text-color), 0.1);
        width: calc(100% + 2rem);
        margin-left: -1rem;
    }
</style>