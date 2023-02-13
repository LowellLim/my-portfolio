<section class="contact">
	<h1 class="contact--title">Get In Touch</h1>
	<p class="contact--desc">
		If you want to contact, ask any question or just to say hi. I will get back to you.
	</p>
	<a
		class="contact--email"
		href="mailto:lowell90@live.com"
		rel="noopener noreferrer"
		target="_blank">Say Hello</a
	>
</section>

<style lang="scss">
	@use '../../styles/global.scss';
	.contact {
		min-height: 50vh;
		max-width: 300px;
		margin: 0px auto 100px;
		text-align: center;
		padding: 100px 0px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		.contact--title {
			color: global.$title-color;
			font-weight: 600;
			font-size: global.$title-font-size;
			margin: 0px 0px 10px;
		}
		.contact--desc {
			color: global.$primary-text-color;
			text-align: center;
		}
	}
	.contact--email {
		display: inline-block;
		color: #bef264;
		background-color: transparent;
		border: 1px solid #bef264;
		border-radius: 4px;
		padding: 1.25rem 1.75rem;
		font-size: 14px;
		font-family: 'SF Mono', 'Fira Code', 'Fira Mono', 'Roboto Mono', monospace;
		line-height: 1;
		text-decoration: none;
		cursor: pointer;
		transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1);
		margin-top: 50px;
		&:hover {
			background-color: #bef264;
            color: #365314;
		}
	}
	@media (min-width: 1024px) {
		.contact {
			min-height: 80vh;
			max-width: 450px;
		}
	}
</style>
