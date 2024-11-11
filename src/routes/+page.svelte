<script>
    import Menu from '$lib/components/Organisms/Menu.svelte';
    import Hero from '$lib/components/Organisms/Hero.svelte';
    import Footer from '$lib/components/Molecules/Footer.svelte';
</script>

<Menu/>
<Hero/>
<Footer/>

<style>

    :global(*) {
        padding: 0;
        margin: 0;
        scroll-behavior: smooth;
    }

    :global(:root) {
        --theme-a: #ff4700;
        --theme-b: #ffcebe;
        --theme-c: #ffece6;
        --bg-a: #0b0e11;
        --bg-b: #1c1e21;
        --bg-c: #1d252e;
        --bg-d: #4a4a55;
        --bg-e: #787b89;
        --fg-a: #ffffff;
        --fg-b: #dfe1e9;
        --fg-c: #c3c4c7;
        --fg-d: #acacb4;
        --fg-e: #5F6377;
        --light-a: #ffffff;
        --light-b: #dfe1e9;
        --light-c: #c3c4c7;
        --light-d: #acacb4;
        --light-e: #5F6377;
        --dark-a: #0b0e11;
        --dark-b: #1c1e21;
        --dark-c: #1d252e;
        --dark-d: #4a4a55;
        --dark-e: #787b89;
    }

    :global(a:not(h1,h2)) {
        color: var(--fg-a);
    }

    :global(a:not(h1,h2):hover) {
        text-decoration-color: var(--theme-a);
        text-decoration-thickness: 0.1rem;
    }

    :global(body) {
        font-family: sans-serif;
        background-color: var(--bg-a);
    }

    :global(h1, h2) {
        text-decoration: none;
    }
    
</style>
