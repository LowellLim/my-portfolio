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
		<a href="https://github.com/LowellLim/my-portfolio" target="blank">
			<span class="sr-only">GitHub</span><svg
				viewBox="0 0 16 16"
				class="icon"
				fill="currentColor"
				aria-hidden="true"
				><path
					d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"
				/>
			</svg>
		</a>
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
	.sr-only {
		position: absolute;
		width: 1px;
		height: 1px;
		padding: 0;
		margin: -1px;
		overflow: hidden;
		clip: rect(0, 0, 0, 0);
		white-space: nowrap;
		border-width: 0;
	}
	.icon {
		width: 1.25rem;
		height: 1.25rem;
		margin-left: 0.5rem;
		color: #eff6ff;
	}
</style>
