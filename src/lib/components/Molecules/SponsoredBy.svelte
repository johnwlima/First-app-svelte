<section class="sponsored-by-container">
    <p>Sponsored by</p>
    <div>
        You! <img class="sponsoredby" src="sponsoredby.svg" alt="#">
    </div>
    <a href="https://opencollective.com/svelte">
        <span>opencollective</span>.com/<span>svelte</span>
    </a>
</section>

<style> 
    
    .sponsored-by-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: var(--fg-a);
        padding: 128px;
    }
    .sponsored-by-container p {
       font-size: 32px;
       font-weight: 100;
       font-family: Arial, Helvetica, sans-serif;
       color: var(--fg-c);
    }

    div {
        color: var(--fg-a);
        font-size: 122px;
        font-weight: 900;
        font-family: Arial, Helvetica, sans-serif;
        letter-spacing: -4px;

        display: flex;
        align-items: center;
    }

    a {
        color: var(--fg-d);
        text-decoration-color: var(--theme-a);
    }
    
    a:hover {
        text-decoration-color: var(--theme-a);
        text-decoration-thickness: 3px;
    }

    a span:first-child {
        color: var(--fg-a);
    }
    
    a span:last-child {
        color: var(--theme-a);
    }

    .sponsoredby {
        height: 100px;
    }
</style>