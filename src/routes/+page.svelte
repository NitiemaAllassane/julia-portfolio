<script>
	import Icon from '@iconify/svelte'
    import { MoveUpRight } from "lucide-svelte";
</script>

<main>
    <!-- section presentation -->
    <section>
        <header>
            <figure>
                <img src="/images/flower.svg" alt="" aria-hidden="true">
            </figure>
        </header>
        <h1>
            Artist Redefining <span>Architecture</span> with AI-Driven Design
        </h1>
    </section>
    <!-- Julia photo -->
    <figure>
        <img src="/images/julia.svg" alt="Julia avatar">
    </figure>

    <section>
        <a href="/">
            <header>
                <div>
                    <p>Musea</p>
                    <span>
                        <MoveUpRight />
                    </span>
                </div>
                <!-- image -->
                 <figure>
                    <img src="/images/image.svg" alt="" aria-hidden="true">
                 </figure>
            </header>
            <ul>
                <li>Elara</li>
                <li>Verve</li>
                <li>Zephyr</li>
            </ul>
        </a>
    </section>

    <section>
        <header>
            <figure>
                <img src="/images/circleIcon.svg" alt="" aria-hidden="true">
            </figure>
        </header>
        <p>
            Julia Huang is an innovative AI artist, renowned for blending 
            cutting-edge technology with creative expression. 
            Based in LA, she crafts unique digital art experiences accessible globally.
        </p>
    </section>

    <!-- contact -->
    <section>
        <header>
            <p>Have some questions ?</p>
            <span>
                <MoveUpRight />
            </span>
        </header>
        <h2>Contact me</h2>
    </section>

    <article>
        <ul>
            <li>
                <a href="/">
                    <Icon icon="simple-icons:instagram" />
                    <!-- <span>Instagram</span> -->
                </a>
            </li>
            <li>
                <a href="/">
                    <Icon icon="simple-icons:x" />
                    <!-- <span>X</span> -->
                </a>
            </li>
            <li>
                <a href="/">
                    <Icon icon="simple-icons:linkedin" />
                    <!-- <span>LinkedIn</span> -->
                </a>
            </li>
        </ul>
    </article>

</main>