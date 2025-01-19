<script lang="ts">
	import ParadiseSpa from '$lib/images/paradise-spa.jpg';
	import SweetIcon from '$lib/images/sweet-icon-laundry.jpg';

	let InnerHeight: number;

	function reveal() {
		let reveals = document.querySelectorAll('.work__wrapper');

		for (let i = 0; i < reveals.length; i++) {
			let elementTop = reveals[i].getBoundingClientRect().top;
			let elementVisible = 200;

			if (elementTop < InnerHeight - elementVisible) {
				reveals[i].classList.add('fadeIn');
			}
		}
	}
</script>

<svelte:window on:scroll={reveal} bind:innerHeight={InnerHeight} />

<section class="work">
	<h1 class="work__title">My Work</h1>
	<p class="work__note">Note: using budget cloud service, first load will be slow</p>
	<div class="work__detail">
		<figure class="work__wrapper work--paradise-background-color">
			<img class="work__thumbnail" src={ParadiseSpa} alt="Paradise Spa Hotel" />
			<figcaption>
				<h3>Paradise SPA Hotel</h3>
				<a
					class="work__button"
					href="https://www.paradisespahotel.com.my"
					target="_blank"
					rel="noreferrer"
					><span>Visit Website</span><span class="icon"
						><svg
							aria-hidden="true"
							focusable="false"
							data-prefix="fas"
							data-icon="angle-right"
							role="img"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 256 512"
							data-fa-i2svg=""
							><path
								fill="currentColor"
								d="M246.6 233.4c12.5 12.5 12.5 32.8 0 45.3l-160 160c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3L178.7 256 41.4 118.6c-12.5-12.5-12.5-32.8 0-45.3s32.8-12.5 45.3 0l160 160z"
								style="--darkreader-inline-fill: currentColor;"
								data-darkreader-inline-fill=""
							/></svg
						></span
					></a
				>
			</figcaption>
		</figure>
		<figure class="work__wrapper work--sweet-icon-background-color">
			<img class="work__thumbnail" src={SweetIcon} alt="Sweet Icon Laundry" />
			<figcaption>
				<h3>Sweet Icon Laundry</h3>
				<a
					class="work__button"
					href="https://www.sweeticonlaundry.com.my"
					target="_blank"
					rel="noreferrer"
					><span>Visit Website</span><span class="icon"
						><svg
							aria-hidden="true"
							focusable="false"
							data-prefix="fas"
							data-icon="angle-right"
							role="img"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 256 512"
							data-fa-i2svg=""
							><path
								fill="currentColor"
								d="M246.6 233.4c12.5 12.5 12.5 32.8 0 45.3l-160 160c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3L178.7 256 41.4 118.6c-12.5-12.5-12.5-32.8 0-45.3s32.8-12.5 45.3 0l160 160z"
								style="--darkreader-inline-fill: currentColor;"
								data-darkreader-inline-fill=""
							/></svg
						></span
					></a
				>
			</figcaption>
		</figure>
	</div>
</section>

<style lang="scss">
	@use '../../styles/global.scss';
	.work {
		min-height: global.$sm-height;
		padding: 5rem;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		&__title {
			font-size: global.$title-font-size;
			color: global.$white-color;
			text-align: center;
		}
		&__detail {
			display: grid;
			align-items: center;
			justify-items: center;
			gap: 2rem;
			margin-top: 5rem;
			margin-left: auto;
			margin-right: auto;
			max-width: 1536px;
		}
		&__note {
			color: global.$light-grey;
		}
	}

	.work__wrapper {
		opacity: 0;
		text-align: center;
		min-width: 200px;
		max-width: 400px;
		position: relative;
		overflow: hidden;
		border-radius: 1rem;
		box-shadow: 0 0 0 2px #262626;
		height: 100%;
		&:hover img {
			transform: scale(1.1);
		}
		&:hover figcaption {
			background-color: #171717;
			opacity: 1;
		}
		&::before,
		&::after {
			content: '';
			display: block;
			width: 100%;
			height: 100%;
			position: absolute;
			top: 0;
			left: 0;
			z-index: 1;
		}
	}

	.work--paradise-background-color {
		&::after {
			background: #64748b;
			mix-blend-mode: multiply;
		}
	}
	.work--sweet-icon-background-color {
		&::after {
			background: #6acebb;
			mix-blend-mode: multiply;
		}
	}
	.work__thumbnail {
		background-size: cover;
		background-position: center;
		transform: scale(1);
		transition: 0.25s ease-in-out;
		position: relative;
		filter: contrast(0.7);
	}
	figcaption {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		opacity: 1;
		transition: 0.45s ease-in-out;
		z-index: 2;
	}
	.work__button {
		margin: 0 auto;
		font-size: 18px;
		padding: 1.2rem;
		font-weight: 400;
		display: inline-flex;
		justify-content: center;
		align-items: center;
		border: 2px solid #6e07f3;
		color: white;
		height: 2.5rem;
		white-space: nowrap;
		border-radius: 9999px;
		cursor: pointer;
		text-decoration: none;
		background-color: #6e07f3;
		.icon {
			display: inline-flex;
			justify-content: center;
			height: 1.5rem;
			width: 1.5rem;
			margin-top: 4px;
			margin-left: 0px;
		}
	}
	h3 {
		color: #a8a29e;
	}

	@media (min-width: 1024px) {
		.work {
			min-height: global.$md-height;
			&__detail {
				grid-template-columns: repeat(3, 1fr);
			}
		}

		figcaption {
			opacity: 0;
		}
		.work__button {
			background-color: initial;
			&:hover {
				background-color: #6e07f3;
			}
		}
	}
</style>
