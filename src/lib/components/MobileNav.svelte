<script>
    import { slide } from 'svelte/transition';
    import { X } from 'lucide-svelte';
    import Icon from '@iconify/svelte';
    import { mobileNav } from '$lib/global state/navbarState.svelte';

    import { afterNavigate } from '$app/navigation';
	afterNavigate(() => mobileNav.isOpened = false);

    function closeMobileNav() {
        if( !mobileNav.isOpened ) return;
        mobileNav.isOpened = false;
    }
</script>


<nav 
    class="md:hidden fixed top-0 left-0 w-full h-[100vh] bg-primary z-40"
    in:slide={{duration: 500}}
    out:slide={{duration: 300}}
>
    <div class="container">
        <header class="flex items-center justify-between py-6 mb-16">
            <a href="/">
                <img src="/images/logo.svg" alt="Logo">
            </a>

            <!-- Close button -->
            <button
                onclick={closeMobileNav}
            >
                <X />
            </button>
        </header>

        <ul class="flex flex-col items-center gap-12 mb-36">
            <li><a href="/" class=" font-light">PROJECTS</a></li>
            <li><a href="/" class=" font-light">ABOUT</a></li>
            <li><a href="/" class=" font-light">CONTACT</a></li>
        </ul>

        <!-- Social links -->
        <ul class="flex items-center justify-center gap-6">
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
    </div>
</nav>