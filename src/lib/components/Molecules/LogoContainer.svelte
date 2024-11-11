<script>
    import Logo from '$lib/components/Atoms/Logo.svelte';
</script>

<a href="http://localhost:5173/#hero" class="logo-container">
    <Logo/>
    <p class="logo-text">SVELTEHACK</p>
</a>

<style>
    .logo-text {
        color: white;
        font-family: sans-serif;
        font-size: 20px;
        margin-left: 8px;
        margin-top: 4px;
        font-weight: 400;
    }

    .logo-container {
        display: flex;
        align-items: center;
        margin-right: 16px;
        text-decoration: none;
    }
</style>