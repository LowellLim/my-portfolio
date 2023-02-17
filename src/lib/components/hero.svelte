<script lang="ts">
	import KeyboardMouse from '$lib/images/keyboard-mouse.jpg';
</script>

<section class="hero">
	<img class="hero__image" src={KeyboardMouse} alt="Keyboard Mouse" />
	<div class="hero__intro">
		<div>
			<header>
				<h1 class="intro--white intro__title">Hello World!</h1>
				<h3 class="intro--red intro--animation">- I am</h3>
				<h1 class="intro__name intro--white  intro--animation">Lowell Lim</h1>
				<h3 class="intro--red intro--animation">Full Stack Developer</h3>
			</header>
			<p class="intro__desc intro--animation">
				I am a full-stack developer in Malaysia, have develop and maintain Web, Mobile, Desktop apps
				and services. Previously was a C# .NET Developer worked with a few companys, and is
				switching to Javascript/Typescript.
			</p>
		</div>
	</div>
</section>

<style lang="scss">
	@use '../../styles/global.scss';

	.hero {
		min-height: global.$sm-height;
		height: global.$sm-height;
		display: flex;
		&__image {
			height: inherit;
			width: 100%;
			filter: opacity(0.1);
			object-fit: cover;
		}
		&__intro {
			position: absolute;
			height: inherit;
			inset: 0;
			display: flex;
			justify-content: center;
			align-items: center;
		}
	}
	.intro--white {
		color: global.$white-color;
		font-weight: 600;
	}
	.intro__name {
		font-size: 400%;
	}
	.intro__title {
		overflow: hidden;
		white-space: nowrap;
		width: 0;
		animation: typing 3s 0.8s steps(30, end) forwards;
	}
	.intro--red {
		color: global.$secondary-text-color;
	}

	.intro__desc {
		color: global.$white-color;
		max-width: 350px;
		text-align: left;
		line-height: 1.75rem;
	}
	.intro--animation {
		opacity: 0;
		@include global.fadeIn(2s, 0.8s);
	}
	@keyframes typing {
		from {
			width: 0;
		}
		to {
			width: 100%;
		}
	}

	@media (min-width: 1024px) {
		.hero {
			flex-direction: row;
			min-height: global.$md-height;
			height: global.$md-height;
			&__intro {
				position: initial;
				width: 100%;
			}
		}
		.intro__desc {
			color: global.$primary-text-color;
			max-width: 450px;
		}
	}
</style>
