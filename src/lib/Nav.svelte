<script lang="ts">
    import NameEasterEgg from "./NameEasterEgg.svelte";
</script>


<nav>
    <div>
        <span class="logo">
            <NameEasterEgg />
        </span>
        <a href="https://github.com/thisisniea" target="_blank" rel="noreferrer" style="--color: 64, 120, 192;">GitHub</a>
        <a href="https://discord.com/users/753760071724302476" target="_blank" rel="noreferrer" style="--color: 114, 137, 218;">Discord</a>
        <a href="https://youtube.com/@this-is-niea" target="_blank" rel="noreferrer" style="--color: 255, 0, 0;">YouTube</a>
    </div>
    <hr>
</nav>

<style>
    nav {
        position: fixed;
        top: 3px;
        left: 0;
        width: 100%;
        height: 3rem;
        border-bottom: 1px solid rgba(127, 127, 127, 0.1);
        background-color: rgba(var(--background-color), 0.8);
        backdrop-filter: blur(10px);
        z-index: 1;
    }

    hr {
        position: absolute;
        top: -3px;
        left: 0;
        width: 100%;
        height: 3px;
        margin: 0;
        padding: 0;
        border: none;
        background: linear-gradient(90deg, hsla(195, 69%, 54%, 1) 0%, hsla(228, 54%, 64%, 1) 20%, hsla(283, 55%, 59%, 1) 40%, hsla(318, 50%, 60%, 1) 60%, hsla(34, 47%, 62%, 1) 80%, hsla(68, 76%, 55%, 1) 100%);
    }

    div {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        max-width: 1000px;
        margin: 0 auto;
        padding: 0 1rem;
    }

    .logo {
        margin-left: 0.75rem;
        margin-right: auto;
        user-select: none;
        transform: skewX(-15deg);
    }

    a {
        text-decoration: none;
        margin-left: 1rem;
        padding: 0.35rem 0.75rem;
        background-color: transparent;
        font-family: Inter, sans-serif;
        font-size: 0.85rem;
        border-radius: 0.25rem;
        color: rgba(var(--text-color), 0.8);
        outline: 1px solid rgba(var(--background-color), 0);
    }

    @media (max-width: 600px) {
        a {
            margin-left: .25rem;
        }

        div {
            padding: 0 .5rem;
        }
    }

    a:hover {
        outline: 1px solid rgba(var(--background-color), 0.1);
        outline-color: rgba(var(--text-color), 0.1);
        transition: background-color 0.1s ease-in-out, color 0.1s ease-in-out, outline-color 0.1s ease-in-out;
        color: rgba(var(--text-color), 1);
    }

    @media (prefers-color-scheme: light) {
        a:hover {
            background-color: rgba(var(--color), 0.1);
            outline-color: rgba(var(--color), 0.5);
        }
    }

    @media (prefers-color-scheme: dark) {
        a:hover {
            background-color: rgba(var(--text-color), 0.1);
            outline-color: rgba(var(--color), 0.5);
        }
    }
</style>