<script>
    import Button from '$lib/components/Atoms/Button.svelte';
    import logoContainer from '$lib/components/Molecules/LogoContainer.svelte';
    import MenuIcon from '$lib/components/Atoms/MenuIcon.svelte';
	import LogoContainer from '$lib/components/Molecules/LogoContainer.svelte';
</script>

<header>
    <div class="header-container">
        <div class="header-left-container">
            <!-- logo container -->
            <LogoContainer/>

            <Button 
                Text={"Enter"}
                Hierarchy={"Secondary"}
            />
        </div>

        <MenuIcon/>
    </div>
</header>

<style>

    header {
        background-color: hsla(0, 0%, 50%, 0.1);
        display: flex;
        align-items: center;
        justify-content: center;
        height: 4.5rem;
        position: fixed;
        top: 0;
        width: 100%;
        z-index: 40;
        max-width: 100vw;
        backdrop-filter: blur(20px);
        -webkit-backdrop-filter: blur(20px);
        background: rgba(var(--bg-a-rgb),.75);
        box-shadow: 0 4px 9px #00000012;
        transition: box-shadow .2s ease-in-out;
    }

    .header-container {
        display: flex;
        width: 100%;
        max-width: 1176px;
        padding: 0rem 2rem;

        align-self: center;

        justify-content: space-between;
    }

    .header-left-container {
        display: flex;
        align-items: center;
    }
</style>