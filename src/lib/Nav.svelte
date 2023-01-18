<script lang="ts">
    export let activeNum: number = 0;
</script>


<nav>
    <div>
        <span class="logo">
            <span class="name">niea</span>.me
        </span>
        <button class:active={activeNum === 0} on:click|preventDefault={() => {activeNum = 0}}>Home</button>
        <button class:active={activeNum === 1} on:click|preventDefault={() => {activeNum = 1}}>About</button>
        <button class:active={activeNum === 2} on:click|preventDefault={() => {activeNum = 2}}>Projects</button>
        <button class:active={activeNum === 3} on:click|preventDefault={() => {activeNum = 3}}>Tools</button>
    </div>
    <hr>
</nav>

<style>
    nav {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 3rem;
        border-bottom: 1px solid rgba(127, 127, 127, 0.1);
        background-color: rgba(var(--background-color), 0.8);
        backdrop-filter: blur(10px);
    .name {
        font-weight: bold;
        font-style: italic;
        transform: skewX(-15deg);
        display: inline-block;
    }

    hr {
        position: absolute;
        top: 0;
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
        margin-right: auto;
        user-select: none;
    }

    button {
        margin-left: 1rem;
        padding: 0.35rem 0.75rem;
        border: none;
        background-color: transparent;
        font-family: inherit;
        border-radius: 0.25rem;
    }

    @media (max-width: 600px) {
        button {
            margin-left: .25rem;
        }

        div {
            padding: 0 .5rem;
        }
    }

    button:not(.active) {
        /* 0.8 opacity text */
        color: rgba(var(--text-color), 0.8);
    }

    button:hover {
        background-color: rgba(127, 127, 127, 0.1);
        transition: background-color 0.1s ease-in-out, color 0.1s ease-in-out;
        color: rgba(var(--text-color), 1);
    }

    button.active {
        background-color: rgba(127, 127, 127, 0.2);
    }
</style>