<script>
	import Icon from '@iconify/svelte'
    import { MoveUpRight } from "lucide-svelte";
</script>

<main class="grid grid-cols-1 lg:grid-cols-[3fr_1fr] gap-8 my-6 ">
    <section class="grid grid-cols-1 gap-6">
        <!-- section presentation -->
        <div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3">
            <article class=" bg-primary p-6 rounded-[20px] lg:col-span-2">
                <header class=" mb-16 flex items-center justify-end">
                    <!-- ? animated image -->
                    <figure class=" animate-spin" style="animation-duration: 6s;">
                        <img src="/images/flower.svg" alt="" aria-hidden="true">
                    </figure>
                </header>
                <h1 class="text-5xl md:text-[56px] font-medium">
                    Artist Redefining <span class="font-thin">Architecture</span> with AI-Driven Design
                </h1>
            </article>
            <!-- Julia photo -->
            <figure class=" overflow-hidden rounded-[20px] max-w-fit">
                <img src="/images/julia.svg" alt="Julia avatar">
            </figure>
        </div>

        <div class=" grid grid-cols-1 md:grid-cols-2 gap-6">
            <article class=" bg-primary p-6 rounded-[20px] ">
                <header class="mb-10 md:mb-20">
                    <!-- ? animated image -->
                    <figure class="max-w-fit animate-spin" style="animation-duration: 3s;">
                        <img src="/images/circleIcon.svg" alt="" aria-hidden="true">
                    </figure>
                </header>
                <p class="font-light">
                    Julia Huang is an innovative AI artist, renowned for blending 
                    cutting-edge technology with creative expression. 
                    Based in LA, she crafts unique digital art experiences accessible globally.
                </p>
            </article>

            <!-- contact -->
            <a href="/" class=" block p-6 bg-secondary rounded-[20px] group">
                <header class="flex items-center justify-between mb-16 md:mb-48">
                    <p class="text-[15px] font-light ">Have some questions ?</p>
                    <span class="group-hover:translate-x-1 group-hover:-translate-y-1 transition-transform duration-300">
                        <MoveUpRight />
                    </span>
                </header>
                <h2 class="font-medium">Contact me</h2>
            </a>
        </div>
    </section>

    <!-- * MUSEA -->
    <section class="flex flex-col gap-6">
        <a href="/" class=" block bg-primary rounded-[20px] p-6 hover:bg-secondary transition-colors duration-300 group">
            <header class=" mb-8">
                <div class="flex justify-between items-center mb-5">
                    <p class=" text-2xl font-light">Musea</p>
                    <span>
                        <MoveUpRight />
                    </span>
                </div>
                <!-- image -->
                <figure class=" max-w-full">
                    <img src="/images/image.svg" alt="Preview of Musea digital artwork" class=" w-auto sm:w-full">
                </figure>
            </header>
            <ul>
                <li class="py-6 border-t-2 border-secondary group-hover:border-primary">Elara</li>
                <li class="py-6 border-t-2 border-secondary group-hover:border-primary">Verve</li>
                <li class="py-6 border-t-2 border-secondary group-hover:border-primary">Zephyr</li>
            </ul>
        </a>

        <article class="bg-primary flex items-center justify-center rounded-[20px] p-6 ">
            <ul class="flex items-center gap-6">
                <li>
                    <a href="/" class=" text-2xl">
                        <Icon icon="simple-icons:instagram" />
                        <!-- <span>Instagram</span> -->
                    </a>
                </li>
                <li>
                    <a href="/" class=" text-2xl">
                        <Icon icon="simple-icons:x" />
                        <!-- <span>X</span> -->
                    </a>
                </li>
                <li>
                    <a href="/" class=" text-2xl">
                        <Icon icon="simple-icons:linkedin" />
                        <!-- <span>LinkedIn</span> -->
                    </a>
                </li>
            </ul>
        </article>
    </section>
</main>