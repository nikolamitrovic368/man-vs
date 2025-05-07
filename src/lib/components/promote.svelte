<script lang="ts">
	import miracle from '$lib/assets/miracle.png'
</script>

<div class="promote-container">
	<div class="promote">
		<img src={miracle} alt="Miracle" class="promote-image" />
		<div class="promote-content">
			<h2>
				TARIfF-FREE COMFORT SALE <br />
				<b>GET 20% OFF NOW</b>
			</h2>
		</div>
	</div>
</div>

<style>
	.promote {
		width: 920px;
		display: flex;
		border-radius: 10px;
		background: #fff;
		box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.25);
		margin-left: auto;
		margin-right: auto;
		margin-top: 3rem;
		margin-bottom: 3rem;
	}
	.promote .promote-image {
		width: 350px;
	}
	.promote .promote-content {
		flex: 1 1 0%;
	}
	.promote .promote-content h2 {
		color: var(--primary);
	}
</style>
