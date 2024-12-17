<script>
	import Step from './Step.svelte';

	let steps = [
		{
			name: 'Lightning Bounties',
			icon: 'fa-sharp fa-solid fa-bolt',
			href: 'https://www.lightningbounties.com',
			description:
				'Smoljames Store is a merchandising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.'
		},
		{
			name: 'Cuphead NFT Minting dApp',
			icon: 'fa-solid fa-gamepad',
			href: 'https://aspecta.ai/projects/ef644f95-8422-4f9d-8e86-00f88ae303e7',
			description:
				'Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.'
		},
		{
			name: 'ETH.ID Retro Game Emulator',
			icon: 'fa-brands fa-ethereum',
			href: 'https://boston.me.eth.id/',
			description:
				'Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).'
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
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				Hi! I'm <span class="poppins text-violet-400">Mike </span> Abramo
				<br />Full Stack
				<span class="poppins text-violet-400">Developer</span>
			</h2>
			<p class="text-base sm:text-lg md:text-xl">
				My <span class="text-violet-400"> favorite tech</span> includes JavaScript (NEXT.JS or SvelteKit),
				TailwindCSS, Node.js + Express.js & PostgreSQL or Firebase/Firestore!
			</p>
			<button
				class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
			>
				<div
					class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
				/>
				<h4 class="relative z-9">Get in touch &rarr;</h4>
			</button>
		</div>
		<div class="relative shadow-2xl grid place-items-center">
			<img src={'images/profile.png'} alt="Zetane Engine" class="object-cover z-[2] max-h-[70vh]" />
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
					Smoljames Store is a a merchandising store created with <strong class="text-violet-400"
						>Next.js, Commerce.js, Stripe & Node.js + Express.js!</strong
					> Commerce.js is a product CMS and Stripe is used for all transaction handling.
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
					to upload and mint NFTs directly within the app. It features a responsive design with a
					Cuphead-inspired art deco interface and includes functionalities like wallet connectivity
					via the <strong class="text-violet-400">Mumbai Testnet</strong>.
				</p>
			</Step>
			<Step step={steps[2]}>
				<p>
					The Pokédex is a <strong class="text-violet-400">SvelteKit & TailwindCSS</strong>
					web application, hosted on
					<strong class="text-violet-400">Netlify</strong>, that consumes and caches the
					<strong class="text-violet-400">Pokémon API</strong>
					to display all Pokémon information. Gotta catch them all!
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
				A bit <span class="poppins text-violet-400">about</span> me.
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
		<h5 class={' text-2xl sm:text-3xl font-semibold text-center poppins '}>
			The <span class="text-violet-400">Complete</span> Package
		</h5>
		<div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
			<table class="bg-white text-slate-700 rounded text-center">
				<thead class={'border-b border-solid border-slate-200  '}>
					<tr class="">
						<th />
						<th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
						<th class="bg-violet-700 text-white whitespace-nowrap p-4 px-8">Me</th>
					</tr>
				</thead>
				<tbody>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
							>Dedication</td
						>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-green-500" /></td>
					</tr>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
							>Critical Thought</td
						>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-green-500" /></td>
					</tr>
					<tr>
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
							>Interpersonal Skills</td
						>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-green-500" /></td>
					</tr>
					<tr class="border-t border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
							>Programming Ability</td
						>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-green-500" /></td>
					</tr>
				</tbody>
			</table>
		</div>
		<div class="mx-auto -mt-12 italic sm:hidden opacity-50">
			<p>Scroll to see more &rarr;</p>
		</div>
		<p class="mx-auto">So why not invest?</p>
	</section>
</main>
