<script>
	let promise = fetchAdvise();

	async function fetchAdvise() {
		const response = await fetch('https://api.adviceslip.com/advice', {
			headers: {
				Accept: 'text/plain'
			}
		});

		const data = await response.text();
		const blurg = JSON.parse(data);
		console.log(blurg);
		const blag = blurg.slip.advice;
		console.log(blag);

		return blag;
	}

	function handleClick() {
		promise = fetchAdvise();
	}
</script>

<div class="advise">
	<h1>Random Advise</h1>
	{#await promise}
		<p>...waiting</p>
	{:then advise}
		<p>{advise}</p>
	{/await}
	<button on:click={handleClick}>Get advise</button>
</div>
