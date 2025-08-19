---
layout: article
title: Release 2.0
cover: "{{site.baseurl}}/assets/images/article-front.png"
---

<img class="background" src="{{site.baseurl}}/assets/images/article-front.png" />

# Tiled Screen Version 2.0

Second major version of TiledScreen plasmoid.

<!--
## Tiled Tray

<div class="tile rounded blue">
    <div class="grid x2 adaptive stretch-width">
        <div class="flex column spaced">
            <h4> Introducing Tiled Tray </h4>
            <p> Tiled Tray is a new widget in the Tiled Widgets collection. It provides a flexible tile popup that you can turn into any type of Plasmoid using Tiles. </p>
        </div>
        <img src="{{site.baseurl}}/assets/images/v1-tile-menu.png" />
    </div>
</div>
-->

## Features

<div class="tile rounded purple">
    <div class="grid x2 adaptive stretch-width">
        <img src="{{site.baseurl}}/assets/images/screenview.png" />
        <div class="flex column spaced">
            <h4> Expandable tiles </h4>
            <p> Tiles can now switch the current page into a tile provided one to allow for addition functionality. This is already used by the newly included Networks tile to provide a screen for connecting and disconnecting from networks.</p>
        </div>
    </div>
</div>

<div class="tile rounded">
    <div class="grid x2 adaptive stretch-width">
        <div class="flex column spaced">
            <h4> Text Alignment </h4>
            <p> Now you can change the text alignment direction of Icon and Category tiles. </p>
        </div>
        <img src="{{site.baseurl}}/assets/images/alignment.png" />
    </div>
</div>

## Builtin Tiles

<div class="tile rounded purple">
    <div class="grid x2 adaptive stretch-width">
        <img src="{{site.baseurl}}/assets/images/volume.png" />
        <div class="flex column spaced">
            <h4> Brightness and Volume Tiles </h4>
            <p> Brightness and Volume tiles allow you to adjust the respective system configurations. </p>
        </div>
    </div>
</div>

<div class="tile rounded">
    <div class="grid x2 adaptive stretch-width">
        <div class="flex column spaced">
            <h4> System Toggles </h4>
            <p> This release includes a collection of system toggle tiles that allows you to quickly enable and disable system operations. Included are Do Not Disturb, Caffeine ( Stops automatic screen locking ), Bluetooth and Nightlight </p>
        </div>
        <img src="{{site.baseurl}}/assets/images/toggles.png" />
    </div>
</div>

<div class="tile rounded purple">
    <div class="grid x2 adaptive stretch-width">
        <div class="flex column spaced">
            <h4> Networks Tile </h4>
            <p> Network tile provides a way to connect and disconnect from wired and wireless networks. Left click on the tile opens the Network view while a iddle click will toggle it on or off. </p>
        </div>
        <img src="{{site.baseurl}}/assets/images/network.png" />
    </div>
</div>

## API Changes

1. Addition of `expandedView` property. When defined for a tile, the value is used as the expanded page for the tile. For more info, check the [documentation]({{site.baseurl}}/docs#expanded-view)
1. Addition of the `toggleOnActivate` property to prevent widget from closing when a tile is activated. See [Tile Internals]({{site.baseurl}}/docs#tile-internals)

## Bug fixes

1. Fixed the scroll issues in the tile selector, porting it into a more standard dialog.
