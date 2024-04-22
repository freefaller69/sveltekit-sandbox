<script>
    export let heading;
    export let mainText;
</script>

<div class="text-content">
    <h2>{heading}</h2>
    <p>{mainText}</p>
</div>

<style>
    .text-content {
        grid-area: text;
        max-width: 60ch;
    }
</style>