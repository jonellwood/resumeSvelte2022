<script>
	import Hr from '../lib/hr.svelte';
	import dev from '$lib/assets/dev-site-icon.svg';
	import github from '$lib/assets/github-icon.png';
	import contact from '$lib/assets/contact-icon.png';
	import projects from '$lib/assets/projects-icon.jpg';
	import twitter from '$lib/assets/twitter-icon.png';
</script>

<div class="white-box-in-middle-to-look-like-piece-of-paper">
	<div class="top-div-for-decoration">
		<p class="hidden-text-in-top-div">
			IF YOU CAN SEE THIS TEXT YOU ARE PROBABLY VIEWING SOURCE. PLEASE FEEL FREE TO SUBMIT IDEAS TO
			MAKE THIS BETTER.
		</p>
	</div>
	<div class="view">
		<h1>View! As in view other stuff!</h1>
		<table class="view-table">
			<th /><td />
			<td />

			<tr>
				<td
					><a href="https://jonellwood.dev" target="_blank">
						<img src={dev} width="48px" height="48px" alt="dev icon" />
					</a></td
				>
				<td><a href="https://jonellwood.dev" target="_blank">My Dev Site</a></td>
			</tr>
			<tr>
				<td
					><a href="https://github.com/jonellwood" target="_blank">
						<img src={github} width="48px" height="48px" alt="github icon" />
					</a></td
				>
				<td><a href="https://github.com/jonellwood" target="_blank">My Repo</a></td>
			</tr>
			<tr>
				<td
					><a href="https://contact.jonellwood.dev" target="_blank">
						<img src={contact} width="48px" height="48px" alt="contact icon" />
					</a></td
				>
				<td><a href="https://contact.jonellwood.dev" target="_blank">Contact Me</a></td>
			</tr>
			<tr>
				<td
					><a href="https://projects.jonellwood.dev" target="_blank">
						<img src={projects} width="48px" height="48px" alt="projects icon" />
					</a></td
				>
				<td><a href="https://projects.jonellwood.dev" target="_blank">Projects</a></td>
			</tr>
			<tr>
				<td
					><a href="https://twitter.com/thejonellwood" target="_blank">
						<img src={twitter} width="48px" height="48px" alt="twitter icon" />
					</a></td
				>
				<td><a href="https://twitter.com/thejonellwood" target="_blank">Twitter</a></td>
			</tr>
		</table>
	</div>
	<Hr />
</div>

<style>
	.top-div-for-decoration {
		margin-top: 20px;
		margin-bottom: 20px;
		padding-top: 20px;
		padding-bottom: 20px;
		background-color: cornflowerblue;
		color: cornflowerblue;
	}
	.hidden-text-in-top-div {
		display: none;
	}

	.white-box-in-middle-to-look-like-piece-of-paper {
		background-color: white;
		margin-left: 30px;
		padding-left: 25px;
		margin-right: 30px;
		padding-right: 25px;
		border: 1px black solid;
		height: 1000px;
	}
	.view {
		margin-top: 2rem;
		margin-left: 1rem;
	}
	.view-table th {
		padding-right: 250px;
	}
	a {
		text-decoration: none;
		color: inherit;
	}
</style>
