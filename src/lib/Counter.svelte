<script>
	let count = 0;
	const increment = () => {
		count++;
	};
</script>

<template>
	<button on:click={increment}>
		Clicks: {count}
	</button>
</template>

<style style lang="postcss">
	button {
		font-size: inherit;
		font-family: inherit;
		cursor: pointer;
		font-variant-numeric: tabular-nums;

		/* Using Tailwind classes directly on your HTML elements is recommended over @apply. */
		@apply py-4 px-8;
		@apply text-red-500;
		@apply bg-red-500 bg-opacity-10;
		@apply rounded-full;
		@apply border-2 border-transparent;
		@apply outline-none;
		@apply w-48;
	}

	button:focus {
		@apply border-opacity-100;
	}

	button:active {
		@apply bg-red-500 bg-opacity-20;
	}
</style>
