<script>
    import TitleContainer from '$lib/components/Molecules/TitleContainer.svelte';
    import Button from '$lib/components/Atoms/Button.svelte'
</script>

<main id="hero" class="hero">
    <TitleContainer/>

    <div class="subtitle">
        <div class="text-container">     
            <p class="p1">A Svelte Hackthon </p>
            <p class="p2">[ with not-so-svelte prizes ]</p>
        </div>

        <Button
            Text = {"Learn more about Svelte"}
            Hierarchy = {"Primary"}
        />
    </div>
</main>

<style>
    .hero {
        height: 100vh;
        display: flex;
        flex-direction: column;
        align-items: top;
        max-width: 1176px;
        margin: 0 auto;
        padding: 120px 40px;
    }
    
    .subtitle {
        display: flex;
        flex-direction: column;
        gap: 1rem;
        margin-top: 2rem;
    }
    
    .text-container {
        display: inline;
    }
    
    .p1 {
        color: var(--light-c);
        font-size: 1.75rem;
        font-weight: 400;
        line-height: 140%;
    }
    
    .p2 {
        color: var(--light-e);
        font-size: 1.125rem;
        font-weight: 400;
        letter-spacing: 1.25px;
    }
</style>