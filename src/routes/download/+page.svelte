<script lang="ts">
	import Overlain from '$lib/components/Overlain.svelte';
	import Tile from '$lib/components/Tile.svelte';
</script>

<Overlain>
	<h1>Download</h1>
	<div class="row mob-col equal">
		<Tile
			title="Plasma Get New"
			description="Automatic installation. Recommended"
			color="purple"
			link="#plasmagetnew"
		/>
		<Tile
			title="KDE (Pling) Store (Tiled Screen)"
			description="Install manually. "
			color="blue"
			link="https://store.kde.org/p/2238981"
			external
		/>
		<Tile
			title="KDE (Pling) Store (Tiled Launcher)"
			description="Install manually. "
			color="light"
			link="https://www.pling.com/p/2328139/"
			external
		/>
	</div>
	<a id="plasmagetnew">
	<h2> Plasma Get New </h2>
	</a>
	<div class="details">
		<p>Use KDE Plasma's built in "Get New Widgets" dialog to install and update one of Tiled Widgets</p>
		<ol>
			<li><b>Right Click</b> on an empty space on the Desktop</li>
			<li>Enter <i>Edit Mode -> Add or Manage Widgets -> Get New -> Download new...</i></li>
			<li>Search for <b>Tiled Screen</b></li>
			<li>Click <i>Download</i> and select the latest version</li>
		</ol>
		<p>You can update widgets later using the same steps.</p>
	</div>
	<h2> From Source </h2>
	<div class="details">
		<p>If you want to test tiled screen or wants to have the latest development build, you would need to install it from the source.</p>
<pre style='color:#cad3f5;background-color:rgba(36,39,58,0.745098);font-size: 12pt;padding: 2ch;border-radius: 0.5ch; overflow-x: scroll;'>
<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>cd</span></i> path/to/save/source

<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>git</span></i> clone --recurse-submodules https://github.com/kavinunethsara/tiledscreen

<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>cd</span></i> tiledscreen
<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>mkdir</span></i> build
<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>cd</span></i> build
<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>cmake</span></i> .. -DCMAKE_INSTALL_PREFIX<span style='color:#91d7e3;'>=</span><i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>HOME</span></i>/.local/
<i><span style='color:#ee99a0;'>$</span></i><i><span style='color:#ee99a0;'>make</span></i> install
</pre>
	</div>
</Overlain>

<style lang="scss">
	@use '/src/sass/units';
	@use '/src/sass/colors';
	.details {
		display: flex;
		flex-direction: column;

		padding: units.$s-lg;

		background-color: colors.$view;
	}
</style>
