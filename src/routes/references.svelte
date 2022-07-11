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
	<div class="references">
		<h1>References</h1>
		<table class="references-table">
			<tr>
				<th>Name</th>
				<th>Email Address</th>
				<th>Phone Number</th>
				<th>Personal or Professional</th>
			</tr>
			<tr>
				<td>Mike Cochran</td>
				<td><a href="mailto:pineymike@yahoo.com">pineymike@yahoo.com</a></td>
				<td><a href="tel:843-696-7550">843-696-7550</a></td>
				<td>Professional</td>
			</tr>
			<tr>
				<td>Wynette DeGroot</td>
				<td
					><a href="mailto:wynette.degroot@cityofhanahan.com">wynette.degroot@cityofhanahan.com</a>
				</td>
				<td><a href="tel:603-490-2539">603-490-2539</a></td>
				<td>Professional</td>
			</tr>
		</table>
	</div>
	<Hr />
</div>

<style>
	.references {
		margin-top: 2rem;
		/* color: red; */
		margin-left: 1rem;
	}
	.references-table th {
		padding-right: 175px;
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
