<script>
	import profileImage from '../images/profile_image.webp';
	import bdaoImage from '../images/BostonDAOlogo.webp';
	import ethBostonLogo from '../images/ethBostonLogo.webp';
	import mitBTCExpoLogo from '../images/mitBTCExpoLogo.webp';
	import lbLogo from '../images/LB_Logo_Dark.webp';
</script>

<footer class="bg-slate-900 text-white py-8 px-4 mt-2">
	<div
		class="max-w-6xl mx-auto flex flex-col md:flex-row sm:flex-row justify-around items-center gap-8"
	>
		<!-- Profile Section -->
		<div class="flex flex-col items-center space-y-4 profile-card md:items-start md:flex-1">
			<div class="flex items-center space-x-4">
				<img
					src={profileImage}
					alt="Mike Abramo"
					class="w-16 h-16 rounded-full border-2 border-violet-400"
					loading="lazy"
				/>
				<div>
					<h3 class="font-bold text-lg">Mike Abramo</h3>
					<p class="text-sm text-gray-400">If it's not decentralized, it's not crypto.</p>
				</div>
			</div>
			<!-- <h3 class="flex flex-col font-bold text-lg">My Orginizations</h3> -->
			<div class="icon-container">
				<div class="icon-item">
					<a href="https://mitbitcoinexpo.org/" target="_blank">
						<img
							src={mitBTCExpoLogo}
							alt="MIT Bitcoin Expo"
							class="w-16 h-16 rounded-full border-2 border-violet-400"
							loading="lazy"
						/>
					</a>
					<p>MIT BTC<br />Expo</p>
				</div>
				<div class="icon-item">
					<a href="https://www.ethboston.xyz/" target="_blank">
						<img
							src={ethBostonLogo}
							alt="Boston DAO"
							class="w-16 h-16 rounded-full border-2 border-violet-400"
							loading="lazy"
						/>
					</a>
					<p>ETH<br /> Boston</p>
				</div>
				<div class="icon-item">
					<a href="https://x.com/thebostondao" target="_blank">
						<img
							src={bdaoImage}
							alt="Boston DAO"
							class="w-16 h-16 rounded-full border-2 border-violet-400"
							loading="lazy"
						/>
					</a>
					<p>Boston<br /> DAO</p>
				</div>
				<div class="icon-item">
					<a href="https://www.lightningbounties.com/" target="_blank">
						<img
							src={lbLogo}
							alt="Lightning Bounties"
							class="w-16 h-16 rounded-full border-2 border-violet-400"
							loading="lazy"
						/>
					</a>
					<p>Lightning<br /> Bounties</p>
				</div>
			</div>
		</div>

		<div class="container mx-auto px-4 pl-4 md:pl-8 lg:pl-16">
			<!-- Navigation Links -->
			<div class="flex-1 space-y-4 text-center md:text-center">
				<h3 class="flex items-center text-lg font-semibold mb-4 text-violet-400">Quick Links</h3>
				<div class="flex-1 flex-col space-y-2">
					<a href="#projects" class=" flex items-center hover:text-violet-400 transition-colors"
						><i class="fa-solid fa-code mr-2" />Projects
					</a>
					<a class="flex items-center hover:text-violet-400 transition-colors" href="#about">
						<i class="fa-regular fa-circle-user mr-2" />
						About
					</a>
					<a
						href="https://blog.lightningbounties.com/"
						class="flex items-center hover:text-violet-400 transition-colors"
						target="_blank"
					>
						<i class="fa-solid fa-pencil mr-2" />
						Blog
					</a>
				</div>
			</div>

			<!-- Social Links -->
			<div class="flex-1 space-y-4 text-center md:text-center">
				<h3 class="flex items-center text-lg font-semibold mb-4 text-violet-400">Connect</h3>
				<div class="flex-1 flex-col space-y-2">
					<a
						href="https://github.com/SonnyMonroe"
						target="_blank"
						class="flex items-center hover:text-violet-400 transition-colors"
					>
						<i class="fa-brands fa-github mr-2" /> GitHub
					</a>
					<a
						href="https://www.linkedin.com/in/michael-abramo/"
						target="_blank"
						class="flex items-center hover:text-violet-400 transition-colors"
					>
						<i class="fa-brands fa-linkedin mr-2" /> LinkedIn
					</a>
					<a
						href="mailto:mabramo11@protonmail.com"
						class="flex items-center hover:text-violet-400 transition-colors"
					>
						<i class="fa-solid fa-envelope mr-2" /> Email
					</a>
				</div>
			</div>
		</div>
	</div>

	<!-- Copyright -->
	<div class="mt-8 pt-8 border-t border-gray-800 text-center text-sm text-gray-400">
		<p>&copy; {new Date().getFullYear()} Mike Abramo. All rights reserved.</p>
	</div>
</footer>

<style>
	.profile-card {
		border: 2px solid #7c3aed;
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		padding: 1rem;
		border-radius: 0.5rem;
		background-color: #1e293b;
		width: 100%;
	}
	.icon-container {
		display: flex;
		flex-basis: content;
		flex-direction: row;
		justify-content: space-between;
		margin-top: 1rem;
		width: 100%;
	}
	.icon-item {
		display: flex;
		flex-direction: column;
		align-items: center;
		text-align: center;
		margin: 0.5rem;
	}
	.icon-item img {
		display: flex;
		width: 50px;
		height: 50px;
	}
	.icon-item p {
		margin-top: 0.5rem;
		font-size: 0.75rem;
		color: #9ca3af;
		line-height: 1;
	}
	.container {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		margin-top: 1rem;
		width: 66.6%;
	}
</style>
