<script lang="ts">
	import bg from '$lib/assets/bg.png'
	import ImageWithText from '$lib/components/image-with-text.svelte'
	import Promote from '$lib/components/promote.svelte'
	import Richtext from '$lib/components/richtext.svelte'
</script>

<img alt="The project logo" src={bg} class="banner" />

<Richtext />
<ImageWithText />
<Promote />

<style>
	.banner {
		width: 100%;
		height: 470px;
		object-fit: cover;
		line-height: 0;
	}
</style>
