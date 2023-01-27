<script lang="ts">
	import Header from '$lib/components/header.svelte';
</script>

<title>My Portfolio</title>
<div class="hero">
	<Header />
	<slot />
</div>

<style type="scss">
	.hero {
		--tw-gradient-from: #06b6d4;
		--tw-gradient-to: #3b82f6;
		--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) 25%;
		background-image: linear-gradient(to bottom, var(--tw-gradient-stops));
		height: inherit;
	}
</style>
