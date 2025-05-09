<script lang="ts">
	import bg from '$lib/assets/bg.png'
	import ImageWithText from '$lib/components/image-with-text.svelte'
	import Promote from '$lib/components/promote.svelte'
	import Richtext from '$lib/components/richtext.svelte'
</script>

<div class="banner">
	<img alt="The project logo" src={bg} />
</div>

<Richtext />
<ImageWithText />
<Promote />

<style>
	.banner {
		width: 100%;
		height: 470px;
		overflow: hidden;
	}
	.banner img {
		width: 100%;
		height: 100%;
		object-fit: cover;
		line-height: 0;
		object-position:top left;
	}

	@media (max-width: 768px) {
		.banner {
			height: 227px;
		}
		.banner img {
			height: 270px;
		}
	}
</style>
