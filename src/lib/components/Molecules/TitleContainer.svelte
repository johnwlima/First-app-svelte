<script>
    import RunesEditionNote from '$lib/components/Atoms/RunesEditionNote.svelte';
</script>

<div class="title-container">
    <h1>
        SvelteHack <br>
        <span>2024</span> <RunesEditionNote/>
    </h1>
</div>

<style>
    
    .title-container {
        width: fit-content;
        height: fit-content;
        padding-left: 1rem;
        border-left: 3px solid var(--theme-a)
    }

    h1 {
        color: var(--fg-a);
        font-size: 6rem;
        font-style: italic;
    }

    span {
        font-weight: 100;
    }
    
</style>