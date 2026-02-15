<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import Tile from '$lib/components/Tile.svelte';
	import { base } from '$app/paths';
</script>

<Header
	title="Tiled Widgets"
	subtitle="A collection of highly customizable widgets for KDE Plasma 6."
/>
<Tile
	title="Version 2.2 Release"
	description="See what's new in Tiled Widgets 2.2"
	link="{base}/changelog/"
	color="light"
/>
<div class="row mob-col equal">
	<Tile
		title="Tiled Screen"
		description="A fullscreen launcher that uses a customizable tile grid."
		background="{base}/tscreen.png"
		link="{base}/tiledscreen"
	/>
	<Tile
		title="Tiled Launcher"
		description="A laucher popup with a customizable tile grid."
		color="purple"
		background="{base}/fed.png"
		link="{base}/tiledlauncher"
	/>
</div>
<Tile
	title="Store"
	description="Download and Install additional tile for Tiled Widgets."
	color="dark"
	link="{base}/store"
	aligned
/>
<Tile
	title="Documentation"
	description="API and Developer documentation for developing your own tiles."
	color="blue"
	link="{base}/docs"
	aligned
/>
