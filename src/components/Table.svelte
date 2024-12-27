<div class="table-container">
	<div
		class="tg-wrap md:w-3/3 bg-slate-800 rounded-lg border border-gray-700 overflow-hidden border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
	>
		<table class="tg">
			<tbody>
				<tr>
					<th>Languages</th>
					<td
						><img src="icons/programming_icons/javascript.png" alt="javascript" />JavaScript
					</td><td><img src="icons/programming_icons/python.png" alt="python" />Python</td>
					<td colspan="7" />
				</tr>
				<tr>
					<th>Database</th>
					<td><img src="icons/database_icons/mysql.png" alt="MySQL" />MySQL</td>
					<td><img src="icons/database_icons/posgress.png" alt="posgress" />Posgress</td>
					<td colspan="7" />
				</tr>
				<tr>
					<th>Frontend</th>
					<td> <img src="icons/frontend_icons/html.png" alt="html" />HTML</td>
					<td> <img src="icons/frontend_icons/css3.png" alt="css3" />CSS</td>
					<td> <img src="icons/frontend_icons/reactjs.png" alt="react" />React</td>
					<td> <img src="icons/frontend_icons/nextjs.png" alt="nextjs" />Nextjs</td>
					<td> <img src="icons/frontend_icons/svelte.png" alt="svelte" />Svelte</td>
					<td> <img src="icons/frontend_icons/sass.png" alt="sass" />Sass</td>
					<td> <img src="icons/frontend_icons/bootstrap.png" alt="bootstrap" />Bootstrap</td>
					<td> <img src="icons/frontend_icons/shadcn.png" alt="shadcn" />ShadCN UI</td>
					<td> <img src="icons/frontend_icons/tailwindcss.png" alt="tailwindcss" />TailwindCSS</td>
				</tr>
				<tr>
					<th>Web3</th>
					<td><img src="icons/web3_icons/solidity.png" alt="solidity" />Solidity</td>
					<td><img src="icons/web3_icons/web3js.png" alt="web3js" />Web3js</td>
					<td><img src="icons/web3_icons/thirdweb.png" alt="thirdweb" />Thirdweb</td>
					<td><img src="icons/web3_icons/alchemy.png" alt="alchemy" />Alchemy</td>
					<td><img src="icons/web3_icons/ipfs.png" alt="ipfs" />IPFS</td>
					<td colspan="4" />
				</tr>
				<tr>
					<th>Docs</th>
					<td><img src="icons/documentation_icons/markdown.png" alt="markdown" />Markdown</td>
					<td><img src="icons/documentation_icons/gitbook.png" alt="gitbook" />Gitbook</td>
					<td><img src="icons/documentation_icons/excalidraw.png" alt="excalidraw" />Excalidraw</td>
					<td><img src="icons/documentation_icons/draw.png" alt="draw" />Draw.io</td>
					<td colspan="5" />
				</tr>
				<tr>
					<th>Design</th>
					<td><img src="icons/design_icons/figma.png" alt="figma" />Figma</td>
					<td><img src="icons/design_icons/canva.png" alt="canva" />Canva</td>
					<td><img src="icons/design_icons/phopedia.png" alt="phopedia" />Phopedia</td>
					<td><img src="icons/design_icons/penpot.png" alt="penpot" />Penpot</td>
					<td><img src="icons/design_icons/simpleicons.png" alt="simpleicons" />Simple Icons</td>
					<td><img src="icons/design_icons/svg.png" alt="svg" />SVG</td>
					<td><img src="icons/design_icons/giphy.png" alt="giphy" />Giphy</td>
					<td colspan="2" />
				</tr>
				<tr>
					<th>Tools</th>
					<td><img src="icons/tools_icons/notion.png" alt="notion" />Notion</td>
					<td><img src="icons/tools_icons/googleslides.png" alt="googleslides" />Google Slides</td>
					<td><img src="icons/tools_icons/perplexity.png" alt="perplexity" />Perplexity</td>
					<td><img src="icons/tools_icons/codepen.png" alt="codepen" />Codepen</td>
					<td><img src="icons/tools_icons/converto.png" alt="converto" />Converto</td>
					<td
						><img src="icons/tools_icons/internet_archive.png" alt="internetarchive" />Internet
						Archive</td
					>
					<td colspan="4" />
				</tr>
				<tr>
					<th>Other</th>
					<td><img src="icons/misq_icons/git.png" alt="git" />Git</td>
					<td><img src="icons/misq_icons/github.png" alt="github" />Github</td>
					<td><img src="icons/misq_icons/bash.png" alt="bash" />Bash</td>
					<td><img src="icons/misq_icons/vercel.png" alt="vercel" />Vercel</td>
					<td><img src="icons/misq_icons/vite.png" alt="vite" />Vite</td>
					<td colspan="5" />
				</tr>
			</tbody>
		</table>
	</div>
</div>

<style>
	.table-container {
		background-color: #1e293b; /* Set background color */
		border-radius: 15px; /* Rounded corners */
	}

	@media screen and (max-width: 767px) {
		.tg {
			width: 90%; /* Use full width on small screens */
			border-spacing: 0; /* Remove spacing for smaller screens */
		}
		.tg-wrap {
			overflow-x: auto;
			-webkit-overflow-scrolling: touch;
		}
	}

	.tg {
		border-collapse: collapse;
		border-color: #a78aff;
		border-spacing: 0; /* Remove default spacing for better control */
		font-family: 'Poppins', sans-serif;
		width: 40%; /* Set a default width */
		margin: 0 auto; /* Center the table */
	}

	.tg th,
	.tg td {
		border-color: #fff;
		border-style: solid;
		border-width: 1px;
		padding: 5px 5px;
		text-align: center; /* Center text */
		vertical-align: middle;
	}

	.tg th {
		background-color: #a78aff;
		color: #1e293b;
		font-size: 1.5rem; /* Use relative units for responsiveness */
		font-style: italic;
		font-weight: bold;
	}

	.tg td {
		background-color: #fff;
		color: #1e293b;
		font-size: 1rem; /* Use relative units for responsiveness */
		font-weight: 900;
	}

	.tg td img {
		width: 50px;
		height: 50px;
		margin: auto;
	}

	tr {
		border: 10px solid #1e293b;
		text-align: center;
	}
</style>
