<script>
    import SvelteSocietyIcon from '$lib/components/Atoms/SvelteSocietyIcon.svelte';
</script>

<section>
    <h2>
        <a href="">Svelte Society</a> is excited to bring you <span>SvelteHack <span class="year">2024</span></span>
    </h2>

    <div class="flex">
        <div class="accent-box">
            <div class="accent-box_text">
                <p>On behalf of the Svelte team and community at large, we're inviting you to compete in this event and share your creations with the official release of Svelte 5.</p>

                <p>In turn, we're contributing thousands in cash <a href="#">prizes</a></p>
        
                <p>Read our <a href="#">rules</a> to learn more about how you can participate, and join our <a href="#">Discord channel</a> to stay tuned.</p>
            </div>
        </div>
        <div class="symbol">
            <SvelteSocietyIcon/>
        </div>
    </div>
</section>

<style>
    
    h2 {
        color: var(--fg-a);
        font-weight: 400;
        font-size: 24px;
    }

    section a {
        text-decoration-color: var(--theme-a);
        text-decoration-thickness: 1px;
        transition: ease;
        color: var(--fg-c);
    }
    
    section a:hover {
        color: var(--fg-a);
        text-decoration-thickness: 3px;
    }

    h2 span {
        color: var(--theme-a);
        font-weight: 700;
    }

    h2 span.year {
        font-weight: 100;
    }

    section {
        display: flex;
        flex-direction: column;
        gap: 40px;
        margin: 0 auto;
        padding: 64px 40px;
        align-items: center;
        justify-content: center;
        text-align: center;
        background-color: var(--bg-b);
        outline: 1px solid color-mix(in hsl,var(--theme-a),transparent 75%);
    }

    section p {
        color: var(--fg-a);
        font-size: 20px;
        font-weight: 400;
        line-height: 140%;
    }

    .accent-box {
        display: flex;
        flex-direction: column;
        padding: 2rem;
        background-color: var(--dark-a);
        text-align: left;
        border-radius: 12px;
        max-width: 800px;

        border: 1px solid var(--theme-a);
        position: relative;
    }

    .symbol {
        margin-top: -2rem;
        z-index: 2;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .flex {
        display: flex;
        flex-direction: column;
    }

    .accent-box_text {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }
    
    .accent-box_text p {
        font-size: 18px;
        font-weight: 400;
    }
</style>