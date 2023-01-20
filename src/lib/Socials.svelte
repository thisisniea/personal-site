<script lang="ts">

</script>

<div class="{$$props.class}">
    <a href="https://discord.com/users/753760071724302476" title="Discord" target="_blank" rel="noreferrer" style="--color: #7289da;">
        <i class="fa-brands fa-discord" aria-hidden="true"></i>
    </a>
    <a href="https://youtube.com/@example" title="YouTube" target="_blank" rel="noreferrer" style="--color: #f00;">
        <i class="fa-brands fa-youtube" aria-hidden="true"></i>
    </a>
    <a href="https://github.com/thisisniea" title="GitHub" target="_blank" rel="noreferrer" style="--color: #333;">
        <i class="fa-brands fa-github-alt" aria-hidden="true"></i>
    </a>
</div>

<style lang="postcss">
    div {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        margin: 2rem 0;
        width: min-content;
        gap: 1rem;
    }

    a {
        font-size: 1.2rem;
        color: rgba(var(--text-color), 0.8);
    }

    a:hover {
        color: var(--color);
        transition: color 0.1s ease-in-out;
        transform: scale(1.1);
    }
</style>