<script>
    import '@fontsource-variable/exo-2'
    import '@fontsource-variable/montserrat'
    import '@fontsource/lato'
    import '../styles/reset.css'
    import '../styles/custom-props.css'
</script>

<main>
    <slot />
</main>

<style>
    :global(html) {
        font-family: var(--font-primary), sans-serif;
        background-color: var(--color-background);
        color: var(--color-text);
    }

    :global(h1, h2, h3, h4, h5, h6) {
        font-family: var(--font-emphatic), sans-serif;
        font-style: italic;
        color: var(--color-accent);
    }
</style>