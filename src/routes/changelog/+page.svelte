<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import DetailTile from '$lib/components/DetailTile.svelte';
	import { base } from '$app/paths';
</script>

<Header title="Version 2.2" subtitle="Introducing Tiled Launcher" />

<DetailTile
	title="Even better key navigation"
	description="Tiled Screen and Laucher now support directional arrow keys for tile navigation."
	color="blue"
	direction="right"
/>

<DetailTile
	title="Debug info"
	description="Now the Tile Grid prints any errors to the console, so Tile developers will have a better time debugging their tiles."
	color="black"
	direction="left"
/>
