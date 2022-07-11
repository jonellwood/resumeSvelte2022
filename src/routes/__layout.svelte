<script>
	import '../app.css';
	import Nav from '../lib/nav.svelte';
	import { time, elapsed } from '../stores.js';

	const formatter = new Intl.DateTimeFormat('en', {
		hour12: true,
		hour: 'numeric',
		minute: '2-digit',
		second: '2-digit'
	});
</script>

<div class="black-header-area" />
<div class="top-menu-and-title">
	<p class="auto-save">
		Auto Save
		<label class="switch">
			<input type="checkbox" />
			<span class="slider round" />
		</label>
	</p>
	<div class="icon-container">
		<img src="src/public/save-icon.png" width="24px" height="24px" alt="save icon" />
		<img src="src/public/undo-icon.png" width="24px" height="24px" alt="undo icon" />
		<img src="src/public/expand-down.png" width="12px" height="12px" alt="down icon" />
		<img src="src/public/redo-icon.png" width="24px" height="24px" alt="redo icon" />
		<img src="src/public/double-down.png" width="24px" height="24px" alt="two dowm icon" />
	</div>

	<p>Jon Ellwood - Resume - Last Saved</p>
	<p class="hidden-text">-</p>
	<p>{formatter.format($time)}</p>
	<form class="form form--search">
		<div class="form__field">
			<input type="search" placeholder="Search" />
			<input type="submit" value="Search" />
		</div>
	</form>
	<p class="icon-container-right">
		<img src="src/public/avatar-icon.png" width="24px" height="24px" alt="avatar icon - get it?" />
		<img src="src/public/minimize-icon.png" width="24px" height="24px" alt="minimize-icon" />
		<img src="src/public/maximize-icon.png" width="24px" height="24px" alt="maximize-icon" />
		<img src="src/public/close-icon.png" width="24px" height="24px" alt="close icon" />
	</p>
</div>
<Nav />
<slot />

<style>
	.black-header-area {
		background-color: black;
		height: 50px;
		margin-left: 30px;
		margin-right: 30px;
	}

	.top-menu-and-title {
		display: flex;
		background-color: #185abd;
		margin-bottom: 0;
		color: white;
		margin-right: 30px;
		margin-left: 30px;
		padding-left: 1rem;
		padding-right: 1rem;
		align-items: center;
	}
	.auto-save {
		font-size: 14px;
	}
	/* The switch - the box around the slider */
	.switch {
		position: relative;
		display: inline-block;
		width: 30px;
		height: 17px;
	}

	.switch input {
		opacity: 0;
		width: 0;
		height: 0;
	}

	.slider {
		position: absolute;
		cursor: pointer;
		top: 0;
		left: 0;
		right: 0;
		bottom: 0;
		background-color: #ccc;
		-webkit-transition: 0.4s;
		transition: 0.4s;
	}

	.slider:before {
		position: absolute;
		content: '';
		height: 11px;
		width: 11px;
		left: 4px;
		bottom: 3px;
		background-color: white;
		-webkit-transition: 0.4s;
		transition: 0.4s;
	}

	input:checked + .slider {
		background-color: #2196f3;
	}

	input:focus + .slider {
		box-shadow: 0 0 1px #2196f3;
	}

	input:checked + .slider:before {
		-webkit-transform: translateX(13px);
		-ms-transform: translateX(13px);
		transform: translateX(13px);
	}

	/* Rounded sliders */
	.slider.round {
		border-radius: 34px;
	}

	.slider.round:before {
		border-radius: 50%;
	}

	.icon-container {
		display: flex;
	}
	.icon-container-right {
		position: absolute;
		right: 65px;
	}
	.icon-container img {
		padding-left: 5px;
		padding-right: 5px;
	}
	.icon-container-right img {
		padding-left: 5px;
		padding-right: 5px;
	}

	input {
		background: none;
		border: 0;
		color: #185abd;
		font: inherit;
		margin: 0;
		padding: 0;
	}

	.form__field {
		align-items: center;
		background-color: #a5b8cc;
		border-radius: 0.125em;
		color: #185abd;
		display: flex;
		margin-left: 1rem;
		height: 30px;
		width: 450px;
	}

	.form--search input[type='search'] {
		flex-grow: 1;
		padding-bottom: 0.75em;
		padding-right: 0.75em;
		padding-top: 0.75em;
	}

	.form--search input[type='submit'] {
		background-image: url('https://cdn.rawgit.com/marcobiedermann/playground/master/ui/search/simple-search-bar/dist/assets/images/magnifier.svg');
		background-position: 50%;
		background-repeat: no-repeat;
		background-size: 1.5em;
		order: -1;
		padding: 0.75em;
		text-indent: -999px;
		width: 3em;
	}
	.hidden-text {
		color: #185abd;
	}
</style>
