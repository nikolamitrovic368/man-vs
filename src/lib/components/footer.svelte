<script lang="ts">
	import Logo from './logo.svelte'
</script>

<footer>
	<Logo />
	<div class="footer-info">
		<div class="footer-info__company">
			<div class="title">NOVUS STUDIO LLC</div>
			<div class="footer-info__company-content content">
				<div class="">
					<div>111 Town Square Place</div>
					<div>Suite 1203 PMB 1065</div>
					<div>Jersey City, New Jersey 07310</div>
				</div>
				<div class="">
					<div>1501 Haines St.</div>
					<div>Jacksonville, FL 32206</div>
					<div>(888) 683-4875</div>
				</div>
			</div>
		</div>
		<div class="footer-info__shipping">
			<div class="title">INFO</div>
			<div class="content">
				<div>Shipping Information</div>
				<div>UPS ground 2-7 business days</div>
				<div>Business Licensing Information</div>
				<div>EIN: 83-3059849</div>
			</div>
		</div>
		<div class="footer-info__support"></div>
	</div>
</footer>

<style>
	footer {
		padding: 66px 165px 42px 165px;
		background-color: #e4f2fb;
		color: var(--primary);
	}
	footer .footer-info {
		display: flex;
		justify-content: space-between;
		padding-top: 60px;
	}
	footer .footer-info .title {
		font-size: 12px;
		font-weight: 900;
		padding-bottom: 12px;
		letter-spacing: 2px;
	}
	footer .footer-info .content {
		line-height: 26px;
		font-size: 14px;
	}
	footer .footer-info .footer-info__company {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}
	footer .footer-info .footer-info__company .footer-info__company-content {
		display: flex;
		gap: 36px;
	}
</style>
