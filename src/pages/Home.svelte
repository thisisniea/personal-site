<script lang="ts">
    // calculate age
    const age = Math.floor((new Date().getTime() - new Date("2003-08-04").getTime()) / 1000 / 60 / 60 / 24 / 365);

</script>

<h1>
    Creative technologist, <br>
    low-level software developer<abbr title="Oxford comma">,</abbr> <br>
    and cat enthusiast.
</h1>

<p>
    I'm Brandon, a {age}-year-old hobbyist developer from The United States. I have a strong interest in all things low-level, including reverse engineering,
    assembly, and operating systems. Aside from that, I also enjoy working on web applications, hence the existence of this website.
</p>

<p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti possimus repellat illo beatae molestias? Voluptatem nobis voluptate rem earum consectetur nisi non inventore, error nesciunt dicta cupiditate, at impedit quia?
    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Perferendis, labore est! V
    luptatem odit quis maxime quas deleniti eveniet facere ratione, voluptatibus consequuntur a, quae, beatae quo doloremque. Deleniti, laborum soluta.
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur eius voluptate, aspernatur temporibus distinctio recusandae molestias voluptatem odio ullam tempore sit? Omnis necessitatibus eum pariatur rerum perferendis in sequi error.
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis ipsum quo inventore eligendi, ea laboriosam laudantium tempora cum 
    vitae harum distinctio in dolorem. Aperiam dolorum molestiae voluptatibus corrupti repellendus quidem?
</p>

<div class="social">
    <a href="https://twitter.com/example">
        <i class="fa fa-twitter" aria-hidden="true"></i>
    </a>
    <a href="https://youtube.com/@example">
        <i class="fa fa-youtube-play" aria-hidden="true"></i>
    </a>
    <a href="https://github.com/thisisniea">
        <i class="fa fa-github" aria-hidden="true"></i>
    </a>
</div>

<hr>

<h3>Spotlight</h3>
<p class="subtitle">A few special projects that you should check out</p>

<div class="spotlight">
    <div class="spotlight-item">
        <img src="https://via.placeholder.com/200/69f/000" alt="placeholder">
        <div class="spotlight-description">
            <h4>Spotlight item 1</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </div>
    <div class="spotlight-item">
        <img src="https://via.placeholder.com/200/cfb/000" alt="placeholder">
        <div class="spotlight-description">
            <h4>Spotlight item 2</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </div>
    <div class="spotlight-item">
        <img src="https://via.placeholder.com/200/ace/000" alt="placeholder">
        <div class="spotlight-description">
            <h4>Spotlight item 3</h4>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod. 
            </p>
        </div>
    </div>
</div>

<style lang="postcss">
    /* horizontal card layout */
    /* eg, one column multi row */
    .spotlight {
        display: grid;
        grid-gap: 1rem;
        margin-top: 1rem;
    }

    .spotlight-item {
        display: flex;
        padding: 1rem;

        background-color: rgba(var(--text-color), 0.1);
        border-radius: 1rem;
        border: 1px solid rgba(var(--text-color), 0.2);
        
        & img {
            width: 100px;
            height: 100px;
            border-radius: 1rem;
            margin-right: 1rem;
        }
    }

    .spotlight-description {

        & h4 {
            margin: 0;
        }

        & p {
            margin-bottom: 0;
        }
    }

    abbr {
        text-decoration: none;
    }

    h1 {
        font-size: 2.5rem;
        margin: 0;
        padding: 0;
        margin-bottom: 2rem;
    }

    @media (max-width: 600px) {
        br {
            display: none;
        }
    }

    p {
        font-weight: light;
        line-height: 1.5rem;
        font-size: .9rem;
        margin-bottom: 1rem;
        color: rgba(var(--text-color), 0.8);
    }

    h3 {
        margin-bottom: 0;
    }

    p.subtitle {
        display: inline;
        font-size: .8rem;
        opacity: 0.8;
    }

    .social {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        margin: 2rem 0;
    }

    .social > a {
        font-size: 1.2rem;
        margin-right: 1rem;
        color: rgba(var(--text-color), 0.8);
    }

    .social > a:hover {
        color: rgba(var(--text-color), 1);
        transition: color 0.1s ease-in-out;
        transform: scale(1.1);
    }

    .social > a:nth-child(1):hover {
        color: #1da1f2;
    }

    .social > a:nth-child(2):hover {
        color: #ff0000;
    }

    .social > a:nth-child(3):hover {
        color: #333333;
    }

    /* ripply line like a sine wave, but with a bit lower frequency */
    hr {
        border: none;
        border-bottom: 1px solid rgba(var(--text-color), 0.1);
        width: calc(100% + 2rem);
        margin-left: -1rem;
    }
</style>