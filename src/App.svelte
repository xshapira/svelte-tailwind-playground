<script>
	import Counter from './lib/Counter.svelte';
	import Tailwindcss from './Tailwindcss.svelte';
</script>

<Tailwindcss />

<template>
	<main>
		<h1>Hello world!</h1>

		<Counter />

		<p>This is a Svelte Template which uses TailwindCSS & comes with Stylelint & Stylelint pre-configured.</p>

		<p>
			<strong class="text-xl text-red-600">Assumes Prettier is already configured.</strong>
		</p>
	</main>
</template>

<style style lang="postcss">
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans',
			'Helvetica Neue', sans-serif;
	}

	main {
		@apply text-center;
		@apply p-4;
		@apply mx-auto;
	}

	h1 {
		@apply text-red-600;
		@apply uppercase;
		@apply text-6xl;
		@apply font-thin;
		@apply leading-tight;
		@apply my-8 mx-auto;
		@apply max-w-xs;
	}

	p {
		@apply max-w-xs;

		margin: 1rem auto;
		@apply leading-snug;
	}

	@screen sm {
		h1 {
			@apply max-w-none;
		}

		p {
			@apply max-w-none;
		}
	}
</style>
