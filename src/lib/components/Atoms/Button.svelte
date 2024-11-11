<script> 
    let {
        href = "https://www.google.com.br/",
        Hierarchy = "Primary",
        Text = "Button"
    } = $props();
    
</script>

<a class={Hierarchy} {href} target="_blank">{Text}</a>

<style>
    .Primary {
        width: fit-content;
        color: var(--fg-d);
        background: var(--bg-a);
        border-radius: 0px;
        border-left: 1px solid transparent;
        padding: 12px 32px;
        letter-spacing: 1.5px;
        font-size: 1rem;
        font-weight: 400;
        outline: 1px solid transparent;
        transition: all .2s;
        transition-behavior: normal;
        transition-duration: 0.2s;
        transition-timing-function: ease;
        transition-delay: 0s;
        transition-property: all;
        text-underline-offset: .25rem;
        text-decoration: underline;
        position: relative;
    }

    .Primary::after {
        content: "";
        position: absolute;
        top: 0px;
        bottom: 0px;
        left: 0px;
        width: 1px;
        height: 80%;
        background-color: 
        color-mix(in hsl, var(--theme-a), transparent 60%);
        transform: scaleX(1);
        transform-origin: left center;
        margin: auto 0px;
        transition: transform 0.2s cubic-bezier(0.23, 1, 0.32, 1);
    }

    .Secondary {
        width: fit-content;
        color: var(--fg-d);
        background: var(--bg-a);
        border-radius: 4px;
        border: 1px solid var(--fg-e);
        text-decoration: none;
        padding: 8px 32px;
        letter-spacing: 1.5px;
        font-size: 1rem;
        font-weight: 400;
        outline: 1px solid transparent;


        transition: all .2s;
        transition-behavior: normal;
        transition-duration: 0.2s;
        transition-timing-function: ease;
        transition-delay: 0s;
        transition-property: all;
    }

    .Primary:hover {
        color: var(--fg-a);
        background: var(--bg-a);
        border-color: var(--theme-a);
        outline-width: 1px;
        outline-color: var(--theme-a);
        border-radius: 4px;
        text-decoration: none;

    }
    
    .Secondary:hover {
        color: var(--fg-a);
        background: var(--bg-a);
        border-color: var(--theme-a);
        outline-width: 3px;
        outline-offset: -3px;
        outline-color: var(--theme-a);
    }
</style>
