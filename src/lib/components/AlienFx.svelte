<script>
	import TextContent from './TextContent.svelte';
	import Media from './Media.svelte';
	import ColorPicker from './ColorPicker.svelte';

	export let textContent;
	export let mediaContent1;
	export let mediaContent2;
</script>

<section>
	<TextContent {...textContent} />
	<Media {...mediaContent1} />
	<Media {...mediaContent2} />
	<ColorPicker />
</section>

<style>
	section {
		outline: 1px solid hotpink;
        aspect-ratio: 21 / 9;
        display: grid;
        grid-template-areas: 'text media controls';
        grid-template-columns: 1fr 2fr 1fr;
        justify-items: center;
        align-items: center;
        padding-inline: 5rem;
	}
</style>
