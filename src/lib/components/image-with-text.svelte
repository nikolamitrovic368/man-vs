<script lang="ts">
	import cardBg1 from '$lib/assets/card-1.png'
	import cardBg2 from '$lib/assets/card-2.png'
	import cardBg3 from '$lib/assets/card-3.png'
	import cardBg4 from '$lib/assets/card-4.png'
	import cardBg5 from '$lib/assets/card-5.jpg'
	import cardBg6 from '$lib/assets/card-6.png'
	const offers = [
		{
			img: cardBg1,
			title: '1. Luxury Sheets Are Being Hit With Tariffs. Ours Aren’t.',
			desc: 'Many premium bedding brands source their materials from overseas—then pass import tariffs directly onto you. Our premium Sheets are designed to deliver luxury, cooling, and cleanliness without the markup. You get the same high-end quality (or better), without the government taking a cut.'
		},
		{
			img: cardBg2,
			title: '2. Space-Age Innovation Without Space-Age Prices',
			desc: 'Our temperature-regulating sheets were inspired by the same materials NASA uses to keep astronauts cool. And thanks to our unique approach to sourcing and manufacturing, you won’t see those savings eaten up by hidden costs or extra duties. Just smarter comfort, built for Earth.'
		},
		{
			img: cardBg3,
			title: '3. Fewer Washes = Lower Water Bills = Big Wins',
			desc: 'Our silver-infused fibers fight bacteria and odors naturally. That means you can wash less, save more, and feel fresher every night. Traditional sheets just can’t compete—and every unnecessary wash is money down the drain.'
		},
		{
			img: cardBg4,
			title: '4. Why Pay 2-3x More For Sheets That Do Less?',
			desc: 'Most "luxury" brands aren’t antibacterial. They don’t regulate temperature. And they certainly don’t offer real savings. Our premium Sheets deliver softness, cleanliness, and cooling in one high-tech package—without tariff bloat.'
		},
		{
			img: cardBg5,
			title: '5. The Hidden Cost of Dirty Sheets? Your Skin.',
			desc: 'Regular sheets trap bacteria that irritate skin and clog pores. Our silver-infused our premium Sheets help reduce up to 99.7% of bacteria growth, making them a game-changer for anyone who wants clearer skin and fewer breakouts.'
		},
		{
			img: cardBg6,
			title: '6. Try Them. Love Them. Or Get Your Money Back.',
			desc: "No fine print. No hassle. No tariffs. If you don’t love our premium fabric sheets after 30 nights of better sleep, we’ll refund every cent. We’re confident you'll never look at regular sheets the same way again."
		}
	]
</script>

{#each offers as offer, i}
	<div class={['image-with-text', i % 2 === 0 && 'image-with-text--odd']}>
		<img src={offer.img} alt={offer.title} />
		<div class="image-with-text__text">
			<h2>{offer.title}</h2>
			<p>{offer.desc}</p>
		</div>
	</div>
{/each}

<style>
	.image-with-text {
		display: flex;
		height: 609px;
	}
	.image-with-text--odd {
		flex-direction: row-reverse;
	}
	.image-with-text img {
		width: 50%;
		object-fit: cover; /* Added to maintain aspect ratio */
	}
	.image-with-text .image-with-text__text {
		width: 50%;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		background-color: var(--primary);
		gap: 16px;
	}
	.image-with-text--odd .image-with-text__text {
		background-color: #e4f2fb;
	}
	.image-with-text .image-with-text__text h2 {
		color: white;
		margin: 0;
		padding-inline: 110px;
		font-size: 38px;
		font-weight: 700;
		line-height: 46px; /* 121.053% */
		letter-spacing: -0.543px;
	}
	.image-with-text--odd .image-with-text__text h2 {
		color: var(--primary);
	}
	.image-with-text .image-with-text__text p {
		color: white;
		margin: 0;
		padding-inline: 110px;
		font-size: 18px;
		font-weight: 400;
	}
	.image-with-text--odd .image-with-text__text p {
		color: #333b47;
	}
	@media (max-width: 768px) {
		.image-with-text {
			flex-direction: column;
			height: auto;
		}
		.image-with-text img {
			height: 350px;
			width: 100%;
		}
		.image-with-text .image-with-text__text {
			width: 100%;
			padding-block: 40px;
		}
		.image-with-text .image-with-text__text h2 {
			padding-left: 34px;
			padding-right: 14px;
			font-size: 32px;
			line-height: 36px; /* 121.053% */
			letter-spacing: -0.6px;
		}
		.image-with-text .image-with-text__text p {
			color: white;
			margin: 0;
			padding-left: 34px;
			padding-right: 34px;
			font-size: 18px;
			font-weight: 400;
		}
		.image-with-text--odd .image-with-text__text p {
			color: #333b47;
		}
	}
</style>
