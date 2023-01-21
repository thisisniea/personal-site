<script lang="ts">
    const languages = [
        "All",
        "JavaScript",
        "TypeScript",
        "Python",
    ]

    let selectedLanguage;

    $: console.log(selectedLanguage ? selectedLanguage : "No language selected");
</script>

<div>
    <div id="filters">
        <div class="filter">
            <label for="lang">Language</label>
            <select id="lang" bind:value={selectedLanguage}>
                {#each languages as lang, i}
                    <option id="lang-{i}">{lang}</option>
                {/each}
            </select>
        </div>
        <div class="filter">
            <label for="filter-2">Filter 2</label>
            <input type="checkbox" id="filter-2" />
        </div>
        <div class="filter">
            <label for="filter-3">Filter 3</label>
            <input type="checkbox" id="filter-3" />
        </div>
    </div>
</div>

<style lang="postcss">
    #filters {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
        align-items: center;
        align-content: center;
    }

    .filter {
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: flex-start;
        align-items: center;
        align-content: center;
    }

    .filter label {
        margin-right: 1rem;
    }
</style>