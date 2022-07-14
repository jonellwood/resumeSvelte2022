<script>
	// let jokeButton = document.querySelector('.getJoke');
	// let jokeHolder = document.querySelector('.joke p');

	let buttonText = [
		'Ugh',
		'🤦‍♂️',
		'I am moving out',
		'Seriously',
		'Stop It',
		'This is why Mom left',
		'That is the worst'
	];
	let promise = fetchJoke();

	async function fetchJoke() {
		const response = await fetch('https://icanhazdadjoke.com/', {
			headers: {
				Accept: 'text/plain'
			}
		});

		const data = await response.text();

		return data;
	}

	function handleClick() {
		promise = fetchJoke();
	}
</script>

<div class="joke">
	<h1>Dad Jokes</h1>
	{#await promise}
		<p>...waiting</p>
	{:then joke}
		<p>{joke}</p>
	{/await}
	<button on:click={handleClick}>Get a Joke</button>
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
