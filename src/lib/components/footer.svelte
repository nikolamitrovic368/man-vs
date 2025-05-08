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
				<div><b>Shipping Information</b></div>
				<div>UPS ground 2-7 business days</div>
				<div><b>Business Licensing Information</b></div>
				<div>EIN: 83-3059849</div>
			</div>
		</div>
		<div class="footer-info__support">
			<div class="title">CUSTOMER SUPPORT</div>
			<div class="content">
				<svg
					width="28"
					height="20"
					viewBox="0 0 28 20"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						d="M24.7021 0C25.3646 0.000122956 26.0003 0.259359 26.4688 0.720703C26.9372 1.1824 27.2002 1.80905 27.2002 2.46191V17.5391C27.2001 18.1916 26.9362 18.8177 26.4678 19.2793C25.9992 19.7408 25.3637 20 24.7012 20H2.49805C1.83549 19.9999 1.19993 19.7409 0.731445 19.2793C0.26301 18.8177 0.000120955 18.1916 0 17.5391V2.46191C0 1.809 0.262897 1.18237 0.731445 0.720703C1.19997 0.25932 1.83549 7.21899e-05 2.49805 0H24.7021ZM1.58594 18.376C1.82137 18.626 2.15175 18.7685 2.49805 18.7695H24.7012V18.7627C25.044 18.7648 25.3731 18.6284 25.6104 18.3848L18.2402 9.89551L15.4043 12.8154C14.9331 13.2996 14.2815 13.5742 13.6006 13.5742C13.0049 13.5741 12.4319 13.364 11.9824 12.9873L11.7979 12.8154L8.7627 9.68945L1.58594 18.376ZM19.1055 8.99316L25.9502 16.8828L25.9512 2.46094C25.9494 2.31352 25.9202 2.16782 25.8662 2.03027L19.1055 8.99316ZM1.33398 2.03125C1.28 2.16877 1.25175 2.31453 1.25 2.46191V16.8281L7.89258 8.78516L1.33398 2.03125ZM2.49805 1.23047C2.43205 1.23154 2.36591 1.23765 2.30078 1.24902L12.7002 11.9531C12.9358 12.1947 13.2607 12.332 13.6006 12.332C13.9406 12.332 14.2665 12.1948 14.502 11.9531L24.8975 1.24902C24.8325 1.23771 24.767 1.23155 24.7012 1.23047H2.49805Z"
						fill="#00207D"
					/>
				</svg>
				<div>hello@miraclebrand.co</div>
			</div>
		</div>
	</div>
	<hr />
	<div class="footer-disclaimer">
		<p>
			<b>Disclaimer</b>: this is an advertisement, using a fictional customer but discussing
			experiences that are common to real customers of Miracle brand.
		</p>
		<p>
			This is an advertisement and not an actual news article, blog, or consumer protection update
		</p>
		<p>
			The story depicted on this site and the person depicted in the story are not actual news.
			Rather, this story is based on the results that some people who have used these products have
			achieved. The results portrayed in the story and in the comments are illustrative, and may not
			be the results that you achieve with these products. This page could receive compensation for
			clicks on or purchase of products featured on this site.
		</p>
	</div>
	<div class="footer-copyright">
		<div class="footer-copyright__text">Copyright 2022. Novus Studio LLC. All rights reserved.</div>
		<div class="footer-links">
			<div class="footer-links__item">Privacy Policy</div>
			<div class="footer-links__item">Care Guide</div>
			<div class="footer-links__item">Terms of Use</div>
		</div>
	</div>
</footer>

<style>
	footer {
		padding: 66px 165px 42px 165px;
		background-color: #e4f2fb;
		color: var(--primary);
	}
	footer hr {
		border-top: 1px solid var(--primary);
		opacity: 0.2;
		margin-top: 25px;
		margin-bottom: 25px;
		display: none;
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
	}
	footer .footer-info .footer-info__company .footer-info__company-content {
		display: flex;
		gap: 36px;
	}
	footer .footer-info .footer-info__support .title {
		text-align: right;
	}
	footer .footer-info .footer-info__support .content {
		display: flex;
		align-items: center;
		gap: 36px;
		font-weight: 900;
		font-size: 22px;
	}
	footer .footer-disclaimer {
		padding-top: 40px;
		color: var(--primary);
		font-size: 12px;
		line-height: 14px;
	}
	footer .footer-copyright {
		padding-top: 32px;
		color: var(--primary);
		font-size: 12px;
		display: flex;
		justify-content: space-between;
	}
	footer .footer-copyright .footer-links {
		display: flex;
		gap: 32px;
	}
	@media (max-width: 768px) {
		footer {
			padding: 50px 19px 60px 26px;
		}
	footer hr {
		display: block;
	}
		footer .footer-info {
			flex-direction: column;
			justify-content: space-between;
			gap: 35px;
			padding-top: 50px;
		}
		footer .footer-info .footer-info__company .footer-info__company-content {
			gap: 60px;
		}
		footer .footer-info .footer-info__support .title {
			text-align: left;
		}
		footer .footer-info .footer-info__support .content {
			gap: 12px;
		}
		footer .footer-disclaimer {
			padding-top: 0px;
		}
		footer .footer-copyright {
			flex-direction: column-reverse;
			gap: 23px;
		}
		footer .footer-copyright .footer-links {
			display: flex;
			gap: 32px;
		}
	}
</style>
