<script lang="ts">
	import Footer from '$lib/components/footer.svelte'
	import Logo from '$lib/components/logo.svelte'

	let { children } = $props()
</script>

<header>
	<Logo />
</header>
{@render children()}
<Footer />

<style>
	:global {
		:root {
			color-scheme: light;
			--primary: #00227d;
			--danger: #dc2c00;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_black-BF64a625c944b08.woff2') format('woff2');
			font-weight: 900;
			font-style: normal;
			font-display: swap;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_bold-BF64a625c9151d5.woff2') format('woff2');
			font-weight: 700;
			font-style: normal;
			font-display: swap;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_medium-BF64a625c84a521.woff2') format('woff2');
			font-weight: 500;
			font-style: normal;
			font-display: swap;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_regular-BF64a625c9311e1.woff2') format('woff2');
			font-weight: normal;
			font-style: normal;
			font-display: swap;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_light-BF64a625c93e709.woff2') format('woff2');
			font-weight: 300;
			font-style: normal;
			font-display: swap;
		}

		@font-face {
			font-family: 'Brandon Grotesque';
			src: url('/fonts/HvDTrial_Brandon_Grotesque_thin-BF64a625c9034b9.woff2') format('woff2');
			font-weight: 100;
			font-style: normal;
			font-display: swap;
		}
	}
	header {
		height: 60px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
