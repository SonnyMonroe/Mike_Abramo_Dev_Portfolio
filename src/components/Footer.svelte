<script>
	import profileImage from '../images/profile_image.jpg';
</script>

<footer class="bg-slate-900 text-white py-8 px-4 mt-20">
	<div
		class="max-w-6xl mx-auto flex flex-col md:flex-row justify-between items-start md:items-center gap-8"
	>
		<!-- Profile Section -->
		<div class="flex flex-col items-center space-y-4 profile-card md:items-start md:flex-1">
			<div class="flex items-center space-x-4">
				<img
					src={profileImage}
					alt="Mike Abramo"
					class="w-16 h-16 rounded-full border-2 border-violet-400"
				/>
				<div>
					<h3 class="font-bold text-lg">Mike Abramo</h3>
					<p class="text-sm text-gray-400">If it's not decentralized, it's not crypto.</p>
				</div>
			</div>
			<div class="icon-container">
				<div class="icon-item">
					<a href="https://example.com" target="_blank">
						<img src="path/to/mit-bitcoin-expo-icon.png" alt="MIT Bitcoin Expo" />
					</a>
					<p>MIT Bitcoin Expo</p>
				</div>
				<div class="icon-item">
					<a href="https://example.com" target="_blank">
						<img src="path/to/eth-boston-icon.png" alt="ETH Boston" />
					</a>
					<p>ETH Boston</p>
				</div>
				<div class="icon-item">
					<a href="https://example.com" target="_blank">
						<img src="path/to/boston-dao-icon.png" alt="Boston DAO" />
					</a>
					<p>Boston DAO</p>
				</div>
				<div class="icon-item">
					<a href="https://example.com" target="_blank">
						<img src="path/to/coding-with-coffee-icon.png" alt="Coding with Coffee" />
					</a>
					<p>Coding with Coffee</p>
				</div>
			</div>
		</div>

		<!-- Navigation Links -->
		<div class="space-y-4 text-center md:flex-1">
			<h4 class="text-lg font-semibold mb-4 text-violet-400">Quick Links</h4>
			<nav class="flex flex-col space-y-2">
				<a href="#projects" class="hover:text-violet-400 transition-colors"
					><i class="fa-solid fa-code mr-2" />Projects</a
				>
				<a href="#about" class="hover:text-violet-400 transition-colors"
					><i class="fa-regular fa-circle-user mr-2" /> About</a
				>
				<a
					href="https://blog.lightningbounties.com/"
					class="hover:text-violet-400 transition-colors"
					><i class="fa-solid fa-pencil mr-2" /> Blog</a
				>
			</nav>
		</div>

		<!-- Social Links -->
		<div class="space-y-4 text-align md:flex-1">
			<h4 class="text-lg font-semibold mb-4 text-violet-400">Connect</h4>
			<div class="flex flex-col space-y-2">
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

	<!-- Copyright -->
	<div class="mt-8 pt-8 border-t border-gray-800 text-center text-sm text-gray-400">
		<p>&copy; {new Date().getFullYear()} Mike Abramo. All rights reserved.</p>
	</div>
</footer>

<style>
	.profile-card {
		border: 2px solid #7c3aed; /* violet-400 */
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		padding: 1rem;
		border-radius: 0.5rem;
		background-color: #1e293b; /* slate-900 */
	}
	.icon-container {
		display: flex;
		justify-content: space-around;
		margin-top: 1rem;
	}
	.icon-item {
		text-align: center;
	}
	.icon-item img {
		width: 40px;
		height: 40px;
	}
	.icon-item p {
		margin-top: 0.5rem;
		font-size: 0.75rem;
		color: #9ca3af; /* gray-400 */
	}
</style>
