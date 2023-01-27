<script lang="ts">
	import navItems from './routes';
</script>

<div class="navbar">
	<div class="navbar__container">
		{#each navItems as item}
			<h4>
				<a class="navbar--item" href={item.href}>{item.label}</a>
			</h4>
		{/each}
	</div>
</div>

<style lang="scss">
	.navbar {
		display: flex;
		justify-content: center;
		.navbar__container {
			display: flex;
			justify-content: space-around;
			align-items: center;
			width: 50vh;
			height: 10vh;
			color: #ecfeff;
		}
	}
	.navbar--item:hover {
		color: #164e63;
        border-bottom: 3px solid #164e63;
	}
</style>
