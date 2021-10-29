<script context="module">
	import { browser, dev } from '$app/env';
	export const hydrate = dev;
	export const router = browser;
	export const prerender = true;
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="content">
	<h1>ABOUT ME</h1>

	<p>
		I got my start writing HTML and CSS in 2002 going through w3schools.com tutorials. My fascination waxed and
		waned over the years while I dipped my toes into Javascript and PHP. It wasn't until I got my hands on my first
		Android SDK in 2009 that I started working on my own real projects. However, as life and work got in the way, I
		wouldn't be able to move into coding professionally for another 10 years.
	</p>
	<br>
	<p>
		I've been writing production code for 3 years now, but ever since that first dip in 2002, I haven't fully quit
		writing code. My personal experience ranges from washing dishes and door security, to managing construction
		projects and servicing oil rigs. My professional exp
	</p>

	<p>
		The <a href="/todos">TODOs</a> page illustrates SvelteKit's data loading and form handling. Try using
		it with JavaScript disabled!
	</p>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
