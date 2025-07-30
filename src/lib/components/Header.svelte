<script>
    import portfolioLogo from '../../../static/images/logo.svg';
    import { AlignJustify } from 'lucide-svelte';
</script>

<header class=" bg-primary flex justify-between items-center py-10 px-6 rounded-[20px] ">
        <a href="/">
            <img src={portfolioLogo} alt="Portfolio logo">
        </a>

        <nav class="hidden md:block">
            <ul class="flex items-center gap-12">
                <li><a href="/" class=" font-light">PROJECTS</a></li>
                <li><a href="/" class=" font-light">ABOUT</a></li>
                <li><a href="/" class=" font-light">CONTACT</a></li>
            </ul>
        </nav>

        <button class="text-2xl font-semi-bold md:hidden">
            <AlignJustify />
        </button>
</header>