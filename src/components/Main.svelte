<script>
	import Step from './Step.svelte';
	import VideoCards from './VideoCards.svelte';
	import Table from './Table.svelte';
	import excalidrawImage from '../images/excalidraw3.svg';

	let steps = [
		{
			name: 'Lightning Bounties',
			icon: 'fa-sharp fa-solid fa-bolt',
			href: 'https://www.lightningbounties.com',
			description:
				"Lightning Bounties uses Bitcoin's Lightning Network to democratize open-source contributions, offering instant payouts for approved GitHub pull requests."
		},
		{
			name: 'Cuphead NFT Minting dApp',
			icon: 'fa-solid fa-gamepad',
			href: 'https://aspecta.ai/projects/ef644f95-8422-4f9d-8e86-00f88ae303e7',
			description:
				'A unique NFT collection celebrating the iconic art style and characters of the beloved run-and-gun video game Cuphead.'
		},
		{
			name: 'ETH.ID Retro Game Emulator',
			icon: 'fa-brands fa-ethereum',
			href: 'https://boston.me.eth.id/',
			description:
				'This project is a simple retro game emulator that allows you to play classic games from various consoles, including GameBoy, N64, Play Station and Classic Arcade Games. Right Inside of your ETH.id Profile.'
		}
	];

	let benefits = [
		{
			metric: '10x',
			name: 'a self-taught blockchain developer',
			description:
				'Growing up in Boston, a city known for its revolutionary history and innovation, I’ve been inspired to forge my own path in the blockchain space. As a self-taught developer, I began with the basics of HTML, CSS, and JavaScript, and have since evolved into a full-stack blockchain developer. Just as the founding fathers laid the groundwork for a new nation, I aim to contribute to the foundation of a decentralized future by continuously expanding my skills and knowledge.'
		},
		{
			name: 'startup co-founder',
			description:
				'I co-founded <a href="https://www.lightningbounties.com" target="_blank"><span class="text-violet-400">Lightning Bounties</a></span> alongside <a href="https://www.linkedin.com/in/willsutton17/" target="_blank"><span class="text-violet-400">Will Sutton</a></span>, <a href="https://www.linkedin.com/in/jegamboafuentes/" target="_blank"><span class="text-violet-400">Enrique Gamboa</a></span>, and <a href="https://www.linkedin.com/in/kononovp/" target="_blank"> <span class="text-violet-400">Pavel Kononov</a></span>. Our platform revolutionizes open-source development by connecting GitHub workflows with instant Bitcoin payments via the Lightning Network. We empower developers worldwide to earn immediate rewards while helping organizations resolve issues faster and more efficiently.'
		},
		{
			name: 'a crypto advocate & educator',
			description:
				'I am passionate about simplifying complex blockchain concepts to help others understand and leverage crypto for financial freedom. Through <a href="https://blog.lightningbounties.com/" target="_blank"><span class="text-violet-400"> writing,</span> <a href="https://youtu.be/yxv3VpxuIFU?si=v3vEqRq9GkumMETQ" target="_blank"><span class="text-violet-400"> public speaking,</span> and <a href="https://youtu.be/IYmS16ruXp8?feature=shared" target="_blank"> <span class="text-violet-400">community engagement,</span> I aim to empower individuals to explore the transformative potential of decentralized technologies. By breaking down barriers to entry, I strive to inspire curiosity and enable others to confidently navigate the Web3 space.'
		}
	];
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
		<div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
			<div class="px-4 sm:px-6 lg:px-8">
				<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
					Hi! I'm <br /><span class="poppins text-violet-400">Mike Abramo </span>
					<br />& I'm a
					<span class="poppins text-violet-400">
						<img
							src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=72&pause=100&color=A78BFA&vCenter=true&random=true&width=820&height=72&lines=Blockchain+Developer;Startup+Co-Founder;Crypto+Researcher;Open+Source+Maxi"
							alt="Typing SVG"
						/>
					</span>
				</h2>
			</div>
			<div class="px-4 sm:px-6 lg:px-8">
				<p class="text-base sm:text-lg md:text-xl">
					<span class="text-violet-400">See any bugs here?</span> My startup,
					<span class="text-violet-400">Lightning Bounties</span>, is ready to pay you real Bitcoin
					for fixing bugs on my website! We also have fresh open bounties every day.
					<span class="text-violet-400">Interested?</span>
					Click the link below to get started with bounty hunting!
				</p>
			</div>
			<div class="px-4 sm:px-6 lg:px-8">
				<a
					href="https://app.lightningbounties.com/"
					aria-label="Solve Bounties & Earn Bitcoin"
					target="_blank"
				>
					<button
						class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
					>
						<div
							class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
						/>

						<h4 class="relative z-9">Bug Bounties &rarr;</h4>
					</button>
				</a>
			</div>
		</div>
		<div class="flex justify-center lg:justify-end">
			<img
				src={excalidrawImage}
				alt="Profile_Image"
				class="hidden md:block object-cover z-[2] max-h-[90vh] md:mx-auto lg:mx-0 px-4 sm:px-6 lg:px-8"
			/>
		</div>
	</section>
	<section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
		<div class="flex flex-col gap-2 text-center">
			<h6 class="text-large sm:text-xl md:text-2xl">A few of my creative endeavors.</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				Curious to <span class="poppins text-violet-400">see</span> my work?
			</h3>
		</div>
		<a
			href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
			target="_blank"
			class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
		>
			<i class="fa-regular fa-circle-play" />
			<p>Watch the video</p>
		</a>
		<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
			<Step step={steps[0]}>
				<p>
					<strong class="text-violet-400">Lightning Bounties </strong> uses Bitcoin's Lightning
					Network to democratize open-source contributions, offering instant payouts for approved
					GitHub pull requests.
					<strong class="text-violet-400"
						>Lightning Bounties is the only Bug Bounty Platform that rewards contributors in native
						Bitcoin without KYC, or installations.
					</strong>
					Lightning Bounties has already gained significant attention and traction. From Winning First
					Prize at the
					<strong class="text-violet-400"> 2024 MIT Bitcoin Hackathon, </strong> to being featured
					on <strong class="text-violet-400"> Bitcoin News! </strong>
				</p>
			</Step>
			<Step step={steps[1]}>
				<p>
					The Cuphead NFT Minter DApp is a unique platform celebrating the iconic art style of the
					beloved video game, Cuphead. Built using <strong class="text-violet-400"
						>React.js,
					</strong>,
					<strong class="text-violet-400">Thirdweb SDK + NFT.Storage </strong> & Deployed on
					<strong class="text-violet-400">IPFS</strong>
					& <strong class="text-violet-400">Shadcn UI, TailwindCSS</strong> this DApp allows users
					to upload and mint NFTs directly within the app. It also includes functionalities like
					wallet connectivity via the <strong class="text-violet-400">Mumbai Testnet</strong>.
				</p>
			</Step>
			<Step step={steps[2]}>
				<p>
					This project is a simple retro game emulator that allows you to play classic games from
					various consoles, including <strong class="text-violet-400">
						GameBoy, N64, Play Station
					</strong>
					and <strong class="text-violet-400">Classic Arcade Games</strong>
					Inside of your <strong class="text-violet-400">ETH.id Profile.</strong>
					It clinched second place at the
					<strong class="text-violet-400">2023 MIT Bitcoin Hackathon</strong>
					showcasing its innovative blend of blockchain and gaming nostalgia.
				</p>
			</Step>
		</div>
	</section>
	<section
		id="about"
		class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
	>
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
		>
			<h6 class="text-large sm:text-xl md:text-2xl">Want to know more?</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				A bit <span class="poppins text-violet-400">about</span> me
			</h3>
		</div>
		<p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am . . .</p>
		<div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
			{#each benefits as benefit, index}
				<div class="flex gap-6 sm:gap-8">
					<p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
						0{index + 1}
					</p>
					<div class="flex flex-col gap-6 sm:gap-8">
						<h3 class="text-2xl sm:text-3xl md:text-5xl">
							{benefit.name}
						</h3>
						<p>{@html benefit.description}</p>
					</div>
				</div>
			{/each}
		</div>
		<!-- <h1 class={' text-2xl sm:text-3xl font-semibold text-center poppins '}>
			The <span class="text-violet-400">Complete</span> Package
		</h1> -->
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
		>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">Spotlight</h3>
			<h6 class="text-large sm:text-xl md:text-2xl">of my</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				<span class="poppins text-violet-400">Greatest</span> Achievements
			</h3>
		</div>
		<VideoCards />
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
		>
			<h6 class="text-large sm:text-xl md:text-2xl">My</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				Developer <span class="poppins text-violet-400">Tool</span> Box
			</h3>
		</div>
		<div class="flex flex-col overflow-x-scroll gap-10 max-w-[900px] mx-auto w-full">
			<!-- <table class="bg-#617184 text-slate-700 rounded text-center" /> -->
			<Table />
		</div>
		<div class="mx-auto -mt-12 italic sm:hidden opacity-50">
			<p>Scroll to see more &rarr;</p>
		</div>
	</section>
</main>
