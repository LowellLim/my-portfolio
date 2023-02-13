<script lang="ts">
	import KeyboardMouse from '$lib/images/keyboard-mouse.jpg';
</script>

<section class="hero">
	<img class="hero--image" src={KeyboardMouse} alt="Keyboard Mouse" />
	<div class="hero--intro">
		<div class="intro--wrapper">
			<header>
				<h1 class="intro--title">Hello World!</h1>
				<h3 class="intro--red">- I am</h3>
				<h1 class="intro--name">Lowell Lim</h1>
				<h3 class="intro--red">Full Stack Developer</h3>
			</header>
			<p class="intro--desc">
				I am a full-stack developer in Malaysia, have develop Web, Mobile, Desktop apps and
				services. Previously was a C# .NET Developer worked with a few companys, and is switching to
				Javascript/Typescript.
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
		.hero--image {
			height: inherit;
			width: 100%;
			filter: opacity(0.1);
			object-fit: cover;
		}
		.hero--intro {
			position: absolute;
			height: inherit;
			inset: 0;
			display: flex;
			justify-content: center;
			align-items: center;
		}
	}
	.intro--title,
	.intro--name {
		color: global.$title-color;
		font-weight: 600;
	}
	.intro--title {
		overflow: hidden;
		white-space: nowrap;
		width: 0;
		animation: typing 3s steps(30, end) forwards;
		animation-delay: 0.8s;
	}
	.intro--red {
		color: global.$secondary-text-color;
	}
	.intro--name {
		font-size: 400%;
	}
	.intro--desc {
		color: global.$title-color;
		max-width: 350px;
		text-align: left;
		line-height: 1.75rem;
	}
	.intro--red,
	.intro--name,
	.intro--desc {
		animation: fadeInAndOut 2s;
		animation-delay: 0.8s;
	}
	@keyframes fadeInAndOut {
		0% {
			display: none;
			opacity: 0;
			transform: translateY(2.1rem);
		}
		1% {
			display: block;
			opacity: 0;
		}
		100% {
			display: block;
			opacity: 1;
			transform: translateY(0);
		}
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
			.hero--intro {
				position: initial;
				width: 100%;
			}
		}
		.intro--desc {
			color: global.$primary-text-color;
			max-width: 450px;
		}
	}
</style>
