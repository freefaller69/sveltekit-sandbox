<script>
	export let srcUrl;
	export let altText;
	export let className;
</script>

<div class="media">
	<img src={srcUrl} alt={altText} class={className} />
</div>

<style>
	.media {
		grid-area: media;
	}

	.zero-g {
		outline: 3px solid lawngreen;
		animation-name: drift, float;
		animation-duration: 15s, 6s;
		animation-timing-function: ease-in-out;
		animation-iteration-count: infinite;
		animation-direction: alternate;
	}

	@keyframes float {
		0% {
			transform: translateY(0px);
		}

		100% {
			transform: translateY(-25px);
		}
	}

	@keyframes drift {
		0%, 100% {
			translate: 0px;
		}

		25% {
			translate: -10px;
		}

		75% {
			translate: 10px;
		}
	}
</style>
