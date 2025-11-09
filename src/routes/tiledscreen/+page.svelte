<script lang="ts">
	import DetailTile from '$lib/components/DetailTile.svelte';
	import Header from '$lib/components/Header.svelte';
	import { base } from '$app/paths';
</script>

<Header
	title="Tiled Screen"
	subtitle="A Configurable Full-screen Launcher with Tiles"
	image="{base}/tscreen-dark.png"
	thumbnail
/>

<DetailTile
	title="Configurable"
	description="
		An application launcher that adapts to your workflow. With configurable tile layout and custom tiles, your application launcher can look and function exactly the way you want.
	"
	thumbnail="{base}/tscreen-conf.png"
/>

<DetailTile
	title="Extensible"
	description="
		Download costum tiles or create your own. TiledWidgets tile system allows you to create tiles that can do anything a plasmoid can right from your application launcher.
	"
	color="dark"
	thumbnail="{base}/tscreen-dark.png"
	direction="right"
/>

<DetailTile
	title="Familiar"
	description="
		Start Screen was an unique feature in Windows 8/8.1. If you are one of the few who found it perfect for your taste you would feel right at home in Tiled Screen.
	"
	color="green"
	thumbnail="{base}/tscreen-front.png"
/>

<DetailTile
	title="Download"
	description="
		Install Tiled Screen on Plasma 6 using built-in Get New Widgets, or download it maually.
	"
	color="light"
	direction="right"
	link="{base}/download"
/>
