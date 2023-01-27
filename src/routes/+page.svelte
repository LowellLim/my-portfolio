<script lang="ts">
	import ProfilePicture from '$lib/images/ProfilePicture.jpg';
</script>

<div class="home">
	<div class="profile-container">
		<img
			class="profile-picture"
			loading="lazy"
			decoding="async"
			src={ProfilePicture}
			alt="ProfilePicture"
		/>
		<h1>Lowell Lim</h1>
		<p>Full Stack Developer</p>
		<p class="about">
			Lowell is a full-stack developer in Malaysia, have develop Web, Mobile, Desktop softwares and
			services. Previously was a C# .NET Developer worked with a few companys, and is switching to
			Javascript/Typescript.
		</p>
	</div>
	<div class="work">
		<div class="work__box">
			<h2>Work</h2>
			<div class="work__container">
				<span>Paradise SPA Hotel: </span>
				<a class="work--url" href="https://paradisespahotel.com.my/" target="blank">
					<span class="sr-only">GitHub</span><svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="icon"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M12 21a9.004 9.004 0 008.716-6.747M12 21a9.004 9.004 0 01-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 017.843 4.582M12 3a8.997 8.997 0 00-7.843 4.582m15.686 0A11.953 11.953 0 0112 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0121 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0112 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 013 12c0-1.605.42-3.113 1.157-4.418"
						/>
					</svg>
				</a>
				<a
					href="https://gitfront.io/r/Lowell/KTtoRxqvNWAB/hotel-frontend/"
					class="work--url"
					target="blank"
				>
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
			<div class="work__container">
				<span>Admin Hotel Booking (In Progress): </span>
				<a
					href="https://gitfront.io/r/Lowell/PiciekEkbSVr/admin-hotel-booking/"
					class="work--url"
					target="blank"
				>
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
			<div class="work__container">
				<span>Client Hotel Booking (In Progress): </span>
				<a
					href="https://gitfront.io/r/Lowell/y55wbLEi87yz/client-hotel-booking/"
					class="work--url"
					target="blank"
				>
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

			<h2>CV</h2>
			<div class="work__container">
				<span>CV: </span>
				<a
					href="https://drive.google.com/uc?export=download&id=1kg5TfLC8mM1PNEDyzkaNT2ZvpnpMCC1t"
					class="work--url"
					target="blank"
				>
					<span class="sr-only">CV</span><svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="icon"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M3 16.5v2.25A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75V16.5M16.5 12L12 16.5m0 0L7.5 12m4.5 4.5V3"
						/>
					</svg>
				</a>
			</div>
			<h2>Bio</h2>
			<div class="bio-container">
				<div><span class="bio-year">1990</span> Born in Malaysia</div>

				<div>
					<span class="bio-year">2014</span> Completed Degree Program Information System Engineering
					at TAR College
				</div>

				<div><span class="bio-year">2014</span> Worked at Cimation Sbn Bhd</div>

				<div><span class="bio-year">2020</span> Worked at WPH Digital Pte Ltd</div>

				<div><span class="bio-year">2021</span> Worked at JTC Corporation</div>

				<div>
					<span class="bio-year">2021 - present</span> Working on projects and learning Javascript/Typescript,
					frameworks (React/Next.js, Svelte/Sveltekit)
				</div>
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	.profile-container {
		height: 30rem;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		color: #ecfeff;
	}
	.profile-picture {
		border-radius: 50%;
		width: 10rem;
		border: 2px solid #ecfeff;
	}
	.about {
		max-width: 34rem;
		line-height: 1.5;
		text-align: center;
	}
	.work__box {
		background-color: #1e40af;
		padding: 1rem 1.5rem;
		box-shadow: 0 3px 6px hsla(0, 0%, 15%);
		box-shadow: 0 2px 4px hsla(0, 0%, 12%);
		border-radius: 1rem;
		line-height: 1.5;
		color: #eff6ff;
		div {
			margin-bottom: 0.5rem;
		}
	}
	.work__container {
		display: flex;
		align-items: center;
		margin-bottom: 0.1rem;
	}
	.work--url {
		color: #94a3b8;
		display: inherit;
		align-items: inherit;
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
		&:hover {
			color: #64748b;
			text-decoration: underline;
		}
	}
	.bio-container div {
		margin-bottom: 0.2rem;
	}
	.bio-container:last-child {
		margin-bottom: 1rem;
	}
	.bio-year {
		font-weight: bold;
		margin-right: 1rem;
	}
	@media (min-width: 640px) {
		.work {
			padding: 5rem;
		}
	}
</style>
