<script lang="ts">
</script>

<title>My Portfolio</title>
<body>
	<slot />
</body>

<style lang="scss">
	@use '../styles/global.scss';
	body {
		background-color: #1a1712;
	}
	:global(.fadeIn) {
		@include global.fadeIn;
	}
</style>
