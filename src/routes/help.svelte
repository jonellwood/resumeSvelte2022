<script>
	import Advise from '../lib/advise.svelte';
	import Hr from '../lib/hr.svelte';
	import Jokes from '../lib/jokes.svelte';
</script>

<div class="white-box-in-middle-to-look-like-piece-of-paper">
	<div class="top-div-for-decoration">
		<p class="hidden-text-in-top-div">
			IF YOU CAN SEE THIS TEXT YOU ARE PROBABLY VIEWING SOURCE. PLEASE FEEL FREE TO SUBMIT IDEAS TO
			MAKE THIS BETTER.
		</p>
	</div>
	<div class="help">
		<div class="wrapper">
			<Jokes />
		</div>
	</div>
	<div class="help">
		<p>
			This is from a fun little course by <a href="https://wesbos.com"><b>Wes Bos </b></a>. And a
			little fun is always helpful right?
		</p>
	</div>
	<Hr />
	<div class="help">
		<div class="wrapper">
			<Advise />
		</div>
	</div>
	<div class="help">
		<p>
			Advise courtesy of <a href="https://api.adviceslip.com/"><b>Advise Slip API</b></a>
		</p>
	</div>
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
	.help {
		margin-top: 2rem;
		margin-left: 1rem;
	}
	a {
		text-decoration: none;
		color: inherit;
	}
</style>
