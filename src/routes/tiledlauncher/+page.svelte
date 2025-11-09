<script lang="ts">
	import DetailTile from '$lib/components/DetailTile.svelte';
	import Header from '$lib/components/Header.svelte';
	import { base } from '$app/paths';
</script>

<Header
	title="Tiled Launcher"
	subtitle="A Launcher with a configurable tile grid."
	image="{base}/fed.png"
	thumbnail
/>

<DetailTile
	title="Configurable"
	description="
		An application launcher that adapts to your workflow. With configurable tile layout and custom tiles, your application laucnher can look and function exactly the way you want.
	"
	thumbnail="{base}/fed.png"
/>

<DetailTile
	title="Not just a Launcher"
	description="
		Extensive configuration options and configurable grid allows Tiled Launcher to be anything — from an Application Launcher to a Dashboard, or even a System Tray.
	"
	color="dark"
	thumbnail="{base}/systray.png"
	direction="right"
/>

<DetailTile
	title="Stylish and Theme-able"
	description="
		Tiled Launcher takes advantage of the theming capabilities of KDE Plamsa. So whatever your colour scheme and the plasma theme would be, Tiled Launcher can fit right in.
	"
	color="green"
	thumbnail="{base}/bicolor.png"
/>

<DetailTile
	title="Download"
	description="
		Install Tiled Launcher on Plasma 6 using built-in Get New Widgets, or download it maually.
	"
	color="light"
	direction="right"
	link="{base}/download"
/>
