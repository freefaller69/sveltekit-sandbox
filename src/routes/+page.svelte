<script>
	import AlienFx from "../lib/components/AlienFx.svelte";

	const textContent = {
		heading: 'Alien FX Lighting',
		mainText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptas voluptates, amet esse vel, magnam ducimus corrupti dolor nobis hic beatae dolore omnis repellat corporis. Praesentium doloribus dolorem rerum ipsam!'
	}

	const mediaContent1 = {
		srcUrl: 'https://unsplash.it/400/600',
		altText: 'A random portrait'
	}

	const mediaContent2 = {
		srcUrl: 'https://unsplash.it/100/150',
		altText: 'A random portrait',
		className: 'zero-g'
	}
</script>

<h1>SvelteKit Sandbox</h1>
<p>This is a sandbox application for evaluating front end approaches with SvelteKit.</p>
<AlienFx {textContent} {mediaContent1} {mediaContent2} />
