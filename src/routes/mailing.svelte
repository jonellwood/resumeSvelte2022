<script>
	import Hr from '../lib/hr.svelte';
</script>

<div class="white-box-in-middle-to-look-like-piece-of-paper">
	<div class="top-div-for-decoration">
		<p class="hidden-text-in-top-div">
			IF YOU CAN SEE THIS TEXT YOU ARE PROBABLY VIEWING SOURCE. PLEASE FEEL FREE TO SUBMIT IDEAS TO
			MAKE THIS BETTER.
		</p>
	</div>
	<div class="mailing">
		<h1>Mailing Options</h1>
		<p>Email: <a href="mailto:jonellwood@gmail.com">jonellwood@gmail.com</a></p>
		<p alt="icon of snail">🐌 mail:</p>
		<p>21 Monte Sano Drive</p>
		<p>Hanahan, SC 29410</p>
		<br />

		<p>I really did not need to add this page - but what else would I put under the mailing tab?</p>
	</div>
	<Hr />
</div>

<style>
	a {
		text-decoration: none;
		color: inherit;
	}
	.mailing {
		margin-top: 2rem;
		margin-left: 1rem;
	}

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
</style>
