<script lang="ts">

</script>

<h3>Spotlight</h3>
<p class="subtitle">A few special projects I think you'd like.</p>

<ul>
    <li>
        <img src="https://via.placeholder.com/200/69f/000" alt="placeholder">
        <div>
            <h4>Spotlight item 1</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </li>
    <li>
        <img src="https://via.placeholder.com/200/cfb/000" alt="placeholder">
        <div>
            <h4>Spotlight item 2</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </li>
    <li>
        <img src="https://via.placeholder.com/200/ace/000" alt="placeholder">
        <div>
            <h4>Spotlight item 3</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </li>
</ul>

<style lang="postcss">
    h3 {
        margin-bottom: 0;
    }

    ul {
        list-style: none;
        padding: 0;
        margin: 1rem 0;
        display: grid;
        grid-gap: 1rem;
    }

    ul > li {
        display: flex;
        padding: 1rem;

        border-radius: 1rem;
        border: 1px solid rgba(127, 127, 127, 0.2);

        background-color: rgba(127, 127, 127, 0);
        box-shadow: 0 0 1rem rgba(0, 0, 0, 0.2);

        transition: transform 0.2s ease-in-out, background-color 0.2s ease-in-out;
    }

    ul > li:hover {
        background-color: rgba(127, 127, 127, 0.1);
        transform: scale(1.01);

        transition: transform 0.2s ease-in-out, background-color 0.2s ease-in-out;
    }

    ul > li > img {
        width: 100px;
        height: 100px;
        border-radius: 1rem;
        margin-right: 1rem;
    }

    ul > li > div > h4 {
        margin: 0;
    }

    ul > li > div > p {
        margin-bottom: 0;
    }
</style>