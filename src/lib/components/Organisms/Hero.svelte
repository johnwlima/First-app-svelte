<script>
    import TitleContainer from '$lib/components/Molecules/TitleContainer.svelte';
    import Button from '$lib/components/Atoms/Button.svelte'
</script>

<main id="hero" class="hero">
    <div class="title-container">
        <div class="title-box">
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
        </div>
        <div class="tridimensional">
            <!-- <iframe title="illustration" src='https://my.spline.design/clonercubesimplecopy-80128d1da0371e567eebd172e3e0c455/' frameborder='0' width='100%' height='100%'></iframe> -->
            
            <iframe title="illustration" src='https://my.spline.design/radialpattern-245a90991868874c57a8bbabc26d572e/' frameborder='0' width='100%' height='100%'></iframe>
        </div>
    </div>
</main>

<style>
    .hero {
        min-height: 100dvh;
        height: fit-content;
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

    .title-box {
        width: fit-content;
    }

    .tridimensional p {
        color:black;
         background-color:gray;
    }
    
    .tridimensional {
        display: flex;
        align-items: center;
        justify-content: center;
        overflow:visible;
        width: 500px;
        height: 600px;
        align-self: center;
        justify-self: center;
    }

    .title-container {
        display: flex;
        flex-wrap: wrap;
        gap: 4rem;
        width: 100%;
    }
</style>