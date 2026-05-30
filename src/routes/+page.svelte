<script lang="ts">
	import { base } from '$app/paths';

	const screenshots = [
		{
			src: 'appstore-01-reading.png',
			alt: 'Reading screen with primary and relating hexagrams'
		},
		{
			src: 'appstore-02-one-page.png',
			alt: 'Single continuous reading page'
		},
		{
			src: 'appstore-03-cast.png',
			alt: 'Traditional coin casting screen'
		},
		{
			src: 'appstore-04-extended.png',
			alt: 'Extended classical commentary screen'
		},
		{
			src: 'appstore-05-archive.png',
			alt: 'Personal archive of previous readings'
		}
	];

	const features = [
		'Traditional coin casting',
		'Manual hexagram input',
		'Short contemporary readings',
		'Extended classical commentary',
		'Personal archive of questions and readings',
		'English and Ukrainian localization',
		'No accounts required',
		'No social features',
		'No feeds',
		'No notifications'
	];
</script>

<svelte:head>
	<title>I Ching: Shape of Momentum</title>
	<meta
		name="description"
		content="A quiet modern reading companion for the I Ching. Cast coins, read the hexagram, and return later to see what keeps returning."
	/>
	<meta property="og:title" content="I Ching: Shape of Momentum" />
	<meta
		property="og:description"
		content="A quiet space for difficult questions. Cast coins, read the hexagram, return later and see what keeps returning."
	/>
</svelte:head>

<main class="page">
	<section class="intro" aria-labelledby="app-title">
		<div class="title-row">
			<p class="glyphs" aria-hidden="true">易經</p>
			<h1 id="app-title">I Ching: Shape of Momentum</h1>
		</div>
		<p class="promo">
			A quiet space for difficult questions.
			<br />
			Cast coins, read the hexagram, return later and see what keeps returning.
		</p>
	</section>

	<section class="screenshots" aria-label="App screenshots">
		{#each screenshots as screenshot}
			<img
				src="{base}/screenshots/{screenshot.src}"
				alt={screenshot.alt}
				width="1242"
				height="2688"
			/>
		{/each}
	</section>

	<section class="description" aria-label="App description">
		<p>Shape of Momentum is a modern reading companion for the I Ching.</p>

		<p>
			Built around calmness rather than distraction, it keeps the entire reading on a single
			continuous page: question, hexagram, transformation, interpretation and archive.
		</p>

		<p>Features:</p>

		<ul>
			{#each features as feature}
				<li>{feature}</li>
			{/each}
		</ul>

		<p>
			Whether the question is about work, relationships, decisions, business, a project or simply
			understanding the shape of the present moment, the reading remains accessible in one place and
			can be revisited later.
		</p>

		<p class="closing">
			One question.
			<br />
			One reading.
			<br />
			One page.
		</p>

		<div class="store-buttons" aria-label="Store links coming soon">
			<button disabled type="button">
				<span>Download on the</span>
				App Store
			</button>
			<button disabled type="button">
				<span>Get it on</span>
				Google Play
			</button>
		</div>
	</section>

	<footer>Copyright 2026 eGGs.gd</footer>
</main>
