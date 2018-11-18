
Getting Started
===============

Setup
-----

Annoto player s is officially available via CDN and npm.

Annoto works out of the box with not only HTML `<script>` tag, but also all major bundlers/packagers/builders, such as Browserify, WebPack, etc.

### NPM

The recomended way to include Annoto player is via npm:

```sh
$ npm install @annoto/player
```

> The package includes full typings and can be used in typescript/ES6/flow projects.

### CDN

```html
<body>
    <annoto-player></annoto-player>

    <script src="https://player.staging.annoto.net/index.js"></script>
</body>
```

To setup the player, please contiue to [Creating a player](#creating-a-player).

Creating a Player
-----------------

Annoto player is exposed as [UMD module](https://github.com/umdjs/umd), meaning it offers compatibility with the most popular script loaders and can be imported as commonjs/amd/es6. If you are not using any standard loader the player will be exposed on window as global variables.

The simplest way to create a player is using the `annotoPlayer()` method:

```ts
import { annotoPlayer, PlayerOptions, PlayerServices } from '@annoto/player';

const options: PlayerOptions;
const services: PlayerServices;

annotoPlayer(document.querySelector('annoto-player'), options, services).then((player: AnnotoPlayer) => {
    loadWidget(player); 

    return this.player.loadSrc({
        src: 'https://www.youtube.com/watch?v=1T9EZi7KJcc',
        type: 'video/youtube'
    });
}).catch((err) => {
    console.error('player setup error: ', err);
});
```

This will create a new [AnnotoPlayer](modules/annotoplayer.md) instance and setup it for usage. After you have the player instance it can be used to load video sources, setup the Annoto widget and much more.

> Notice the `loadWidget(player)` function call, we will implement it when we talk about [setting up the widget](#setup-the-widget). Loading the widget can be done asynchronous like we are doing in the example above.

Player Options
--------------

Annoto Player extends standard [VideoJS options](https://docs.videojs.com/tutorial-options.html) with some advanced functionality, for more details, please refer to the [API](interfaces/annotoplayer.playeroptions.md).

The default options can be [found here](modules/annotoplayer.md#default_player_options).

Player services
---------------

The player accepts a number of [optional services](interfaces/annotoplayer.playerservices.md). The most important one is [AuthProviderApi](interfaces/annotoplayer.authproviderapi.md). For proper Widget Sing Sign On functionality the serive **must** be implemented.

Setup the Widget
----------------

Setting up and loading Annoto Widget is a 2 step process:

```ts
function loadWidget(player: AnnotoPlayer) {
    const options: WidgetOptions;

    return player.setupWidget(options).then(() => {
        return player.loadWidget();
    }).catch((err) => {
        console.error('Annoto widget setup err: ', err);
    });
}
```

1.  First we setup the widget by calling `player.setupWidget(options)`, this is required only once for the lifecyle of the application, but can be safely called multiple types to update/change the [widget options](#interfaces/annotoplayer.widgetoptions.md). When called multiple times, the new provided options will be merged with previous options so you only need to provide the required changes. All the options are optional, but to use the Annoto Widget in production (not in Demo mode), you would need to set the clientId provided by [Annoto](https://annoto.net).
2.  After the widget is setup, we can load it by calling `player.loadWidget()`.

Advanced Workflows
==================

Single Page Applications
------------------------

Single page applications dynamically add and remove DOM elements on a single webpage. To provide solution for the dynamic nature of the applications, the player has api to close the player when elements are removed and load the player into new DOM elements:

```ts
player.setup();
player.close();
player.reset();
player.loadWidget();
player.closeWidget();
```

For more details please refer to the [API](classes/annotoplayer.annotoplayer-1.md).

> If you are an Angular developer, please [contact us](https://annoto.net), and we will provide you with a reference code for [Angular Component](https://angular.io/guide/architecture-components) of Annoto Player.

