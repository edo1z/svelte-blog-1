<script lang="ts">
	import '@milkdown/theme-nord/style.css';
	import './style.css';
</script>

<div id="header">Svelete Blog 1</div>

<div id="container">
	<slot />
</div>

<style>
	div#header {
		padding: 10px;
		font-weight: bold;
		background: #036;
		color: white;
	}

	div#container {
		width: 100%;
		padding: 10px;
		background: #369;
	}
</style>
