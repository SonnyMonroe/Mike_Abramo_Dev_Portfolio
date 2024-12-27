<script>
	// State management for the hamburger menu
	let showMenu = false;

	// Toggle function with debug logging
	const toggleMenu = () => {
		showMenu = !showMenu;
		console.log('Menu toggled:', showMenu);
	};

	// Props for scroll position and navigation tabs
	export let y;
	export let tabs = [
		{
			name: 'Projects',
			link: 'https://aspecta.ai/u/SonnyMonroe',
			icon: 'fa-solid fa-project-diagram'
		},
		{
			name: 'About Me',
			link: '#about',
			icon: 'fa-solid fa-user'
		},
		{
			name: 'Blog',
			link: 'https://medium.com/@mabramo11',
			icon: 'fa-solid fa-blog'
		},
		{
			name: 'Lightning Bounties',
			link: 'https://www.lightningbounties.com',
			icon: 'fa-solid fa-bolt'
		}
	];
</script>

<header
	class={`scroll z-[9] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid relative
        ${
					y > 0 ? 'py-4 bg-slate-950 border-violet-950' : 'py-6 bg-transparent border-transparent'
				} ${showMenu ? 'hidden' : 'flex'}`}
>
	<!-- Logo and Name Section -->
	<div class="flex items-center">
		<!-- <img src="/favicon/favicon-16x16.png" alt="Logo" class="w-8 h-8 mr-2" /> -->
		<h1 class="font-medium text-xl">
			<b class="font-bold poppins">Mike</b> <span class="">Abramo</span>
		</h1>
	</div>

	<!-- Desktop Navigation -->
	<nav class="hidden md:block">
		<ul class="nav-container">
			{#each tabs as { name, link, icon }}
				<li><a href={link} class="nav-link"><i class={icon} />{name}</a></li>
			{/each}
		</ul>
	</nav>

	<!-- Contact Button (Desktop Only) -->
	<a href="mailto:mabramo11@protonmail.com" class="hidden md:block">
		<button
			class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-violet-600 text-white"
		>
			<div
				class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
			/>
			<h4 class="relative z-9">Contact Me</h4>
		</button>
	</a>

	<!-- Hamburger Menu Button (Mobile Only) -->
	<button
		on:click={toggleMenu}
		class="px-1 aspect-square text-xl rounded grid place-items-center cursor-pointer duration-200 md:hidden"
	>
		<i class="fa-solid fa-bars" />
	</button>
</header>

<!-- Mobile Navigation Menu -->
{#if showMenu}
	<div class="absolute top-0 left-0 w-full px-4 pb-4 flex flex-col gap-4 bg-slate-900 shadow z-10">
		<div
			class="flex items-center justify-center gap-4 border-b-[1.5px] border-solid border-indigo-400 py-4 relative"
		>
			<h2 class="text-white text-2xl font-bold">Menu</h2>
			<i
				on:click={toggleMenu}
				class="fa-solid fa-xmark text-3xl cursor-pointer hover:opacity-60 duration-200 text-white absolute right-4"
				role="button"
			/>
		</div>
		{#each tabs as { name, link, icon }}
			<div
				on:click={toggleMenu}
				class="flex items-center justify-center gap-2 text-xl hover:text-violet-400 duration-200 text-white"
			>
				<i class={icon} />
				<a href={link} class="capitalize">{name}</a>
			</div>
		{/each}
		<a href="mailto:mabramo11@protonmail.com" class="w-full">
			<button
				class="bg-indigo-400 text-white text-lg sm:text-xl md:text-2xl font-medium border-2 border-solid border-indigo-200 rounded-lg px-4 py-2 hover:bg-indigo-300 duration-200 text-center w-full"
			>
				Contact Me
			</button>
		</a>
	</div>
{/if}

<style>
	/* Navigation Styles */
	.nav-link {
		font-size: 1.125rem; /* text-lg */
		padding: 0.5rem 1rem;
		transition: color 0.3s ease;
		display: flex;
		align-items: center;
		gap: 0.5rem;
	}

	.nav-link:hover {
		color: #7c3aed; /* violet-400 */
	}

	.nav-container {
		display: flex;
		gap: 1.5rem;
		flex-wrap: wrap;
	}

	/* Mobile Navigation Styles */
	@media screen and (max-width: 767px) {
		.mobile-nav-link {
			font-size: 1.25rem; /* text-xl */
			padding: 0.75rem 1rem;
			display: flex;
			align-items: center;
			gap: 0.75rem;
			transition: color 0.3s ease;
		}

		.mobile-nav-link:hover {
			color: #7c3aed; /* violet-400 */
		}
	}

	/* Responsive Styles for 767px to 917px */
	@media screen and (min-width: 768px) and (max-width: 917px) {
		.header {
			flex-direction: column;
			align-items: center;
			display: none;
		}

		.nav-container {
			flex-direction: column;
			align-items: center;
			display: none;
		}

		.nav-link {
			font-size: 1rem; /* Adjust font size as needed */
			padding: 0.5rem;
		}

		.blueShadow {
			width: 100%;
			text-align: center;
		}
	}
</style>
