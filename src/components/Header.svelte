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
				}`}
>
	<!-- Logo and Name Section -->
	<div class="flex items-center">
		<img src="/favicon/favicon-16x16.png" alt="Logo" class="w-8 h-8 mr-2" />
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
	<button
		class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-violet-600 text-white hidden md:block"
		on:click={() => (document.getElementById('contact-form').style.display = 'block')}
		on:keydown={(event) =>
			event.key === 'Enter' && (document.getElementById('contact-form').style.display = 'block')}
	>
		<div
			class="absolute top-0 right-full w-full h-full bg-violet-600 opacity-20 group-hover:translate-x-full z-0 duration-200"
		/>
		<h4 class="relative z-9">Contact Me</h4>
	</button>

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
	<div class="absolute top-0 left-0 w-full px-4 pb-4 flex flex-col gap-4bg-indigo-400 shadow z-10">
		<div
			class="flex items-center justify-between gap-4 border-b-[1.5px] border-solid border-indigo-400 py-4"
		>
			<h2>Menu</h2>
			<i
				on:click={toggleMenu}
				class="fa-solid fa-xmark text-lg cursor-pointer hover:opacity-60 duration-200"
				role="button"
			/>
		</div>
		{#each tabs as { name, link }}
			<div on:click={toggleMenu}>
				<a href={link} class="text-sm capitalize">{name}</a>
			</div>
		{/each}
		<button
			on:click={() => {
				document.getElementById('contact-form').style.display = 'block';
				toggleMenu();
			}}
			class="bg-indigo-400 text-white text-lg sm:text-xl md:text-2xl font-medium border-2 border-solid border-indigo-200 rounded-lg px-4 py-2 hover:bg-indigo-300 duration-200 text-center"
		>
			Contact Me
		</button>
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
</style>
