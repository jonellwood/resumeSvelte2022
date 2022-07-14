<script>
	let promise = fetchQuote();

	async function fetchQuote() {
		const response = await fetch('https://programming-quotes-api.herokuapp.com/Quotes/random', {
			headers: {
				Accept: 'application/json'
			}
		});

		const data = await response.json();
		// console.log(data);
		const asdf = data.en;
		// console.log(asdf);
		return asdf;
	}

	function handleClick() {
		promise = fetchQuote();
	}
</script>

<div class="quote">
	<h1>Random Programming Quotes</h1>
	{#await promise}
		<p>...waiting</p>
	{:then quote}
		<p>{quote}</p>
	{/await}
	<button on:click={handleClick}>Get Quote</button>
</div>

<style>
	button {
		line-height: 1.5;
		margin: 10px 0 0 0;
	}
	button:hover {
		cursor: pointer;
	}
</style>
