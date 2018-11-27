

# Index

### Classes

* [AnnotoPlayer](../classes/annotoplayer.annotoplayer-1.md)

### Interfaces

* [AuthProviderApi](../interfaces/annotoplayer.authproviderapi.md)
* [PlayerOptions](../interfaces/annotoplayer.playeroptions.md)
* [PlayerServices](../interfaces/annotoplayer.playerservices.md)
* [SecondarySourceObject](../interfaces/annotoplayer.secondarysourceobject.md)
* [SourceObject](../interfaces/annotoplayer.sourceobject.md)
* [TextTrackOptions](../interfaces/annotoplayer.texttrackoptions.md)
* [WidgetOptions](../interfaces/annotoplayer.widgetoptions.md)
* [WidgetUxOptions](../interfaces/annotoplayer.widgetuxoptions.md)

### Type aliases

* [PlayerAspectRatio](annotoplayer.md#playeraspectratio)
* [PlayerEvent](annotoplayer.md#playerevent)
* [PlayerEventCallback](annotoplayer.md#playereventcallback)
* [TextTrackKind](annotoplayer.md#texttrackkind)
* [TextTrackMode](annotoplayer.md#texttrackmode)
* [VideoType](annotoplayer.md#videotype)

### Variables

* [defaultAssetLoader](annotoplayer.md#defaultassetloader)
* [defaultLogger](annotoplayer.md#defaultlogger)

### Functions

* [annotoPlayer](annotoplayer.md#annotoplayer-2)

### Object literals

* [DEFAULT_PLAYER_OPTIONS](annotoplayer.md#default_player_options)

---

# Type aliases

<a id="playeraspectratio"></a>

##  PlayerAspectRatio

**Ƭ PlayerAspectRatio**: * "239:100" &#124; "16:9" &#124; "16:10" &#124; "4:3" &#124; "100:239" &#124; "9:16" &#124; "10:16" &#124; "3:4" &#124; "auto"
*

___
<a id="playerevent"></a>

##  PlayerEvent

**Ƭ PlayerEvent**: * "play" &#124; "pause" &#124; "seeked" &#124; "seeking" &#124; "timeupdate" &#124; "fullscreenchange" &#124; "ratechange" &#124; "volumechange" &#124; "loadedmetadata" &#124; "durationchange" &#124; "progress" &#124; "waiting" &#124; "playing" &#124; "loadstart"
*

___
<a id="playereventcallback"></a>

##  PlayerEventCallback

**Ƭ PlayerEventCallback**: *`function`*

#### Type declaration
▸(arg?: *`any`*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` arg | `any` |

**Returns:** `void`

___
<a id="texttrackkind"></a>

##  TextTrackKind

**Ƭ TextTrackKind**: *`Videojs.TextTrack.Kind`*

___
<a id="texttrackmode"></a>

##  TextTrackMode

**Ƭ TextTrackMode**: *`Videojs.TextTrack.Mode`*

___
<a id="videotype"></a>

##  VideoType

**Ƭ VideoType**: * "video/mp4" &#124; "video/webm" &#124; "video/youtube" &#124; "application/x-mpegURL"
*

___

# Variables

<a id="defaultassetloader"></a>

## `<Const>` defaultAssetLoader

**● defaultAssetLoader**: *[AssetLoader](../classes/services.assetloader.md)* =  new AssetLoader()

___
<a id="defaultlogger"></a>

## `<Const>` defaultLogger

**● defaultLogger**: *[ConsoleLogger](../classes/services.consolelogger.md)* =  new ConsoleLogger()

___

# Functions

<a id="annotoplayer-2"></a>

##  annotoPlayer

▸ **annotoPlayer**(elementOrId: * `string` &#124; `HTMLElement`*, options?: *[PlayerOptions](../interfaces/annotoplayer.playeroptions.md)*, services?: *[PlayerServices](../interfaces/annotoplayer.playerservices.md)*): `Promise`<[AnnotoPlayer](../classes/annotoplayer.annotoplayer-1.md)>

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| elementOrId |  `string` &#124; `HTMLElement`|  Id of HTMLElement or the element DOM element |
| `Optional` options | [PlayerOptions](../interfaces/annotoplayer.playeroptions.md) |  player options |
| `Optional` services | [PlayerServices](../interfaces/annotoplayer.playerservices.md) |  player services |

**Returns:** `Promise`<[AnnotoPlayer](../classes/annotoplayer.annotoplayer-1.md)>
Promise that resolves with the player instance

___

# Object literals

<a id="default_player_options"></a>

## `<Const>` DEFAULT_PLAYER_OPTIONS

**DEFAULT_PLAYER_OPTIONS**: *`object`*

<a id="default_player_options.controls"></a>

###  controls

**● controls**: *`true`* = true

___
<a id="default_player_options.defaultvolume"></a>

###  defaultVolume

**● defaultVolume**: *`number`* = 0.5

___
<a id="default_player_options.playbackrates"></a>

###  playbackRates

**● playbackRates**: *`number`[]* =  [0.75, 1, 1.25, 1.5, 1.75, 2]

___
<a id="default_player_options.playsinline"></a>

###  playsinline

**● playsinline**: *`true`* = true

___
<a id="default_player_options.preload"></a>

###  preload

**● preload**: *`string`* = "auto"

___
<a id="default_player_options.sources"></a>

###  sources

**● sources**: *`undefined`[]* =  []

___
<a id="default_player_options.techorder"></a>

###  techOrder

**● techOrder**: *`string`[]* =  ['html5', 'youtube']

___
<a id="default_player_options.features"></a>

###  features

**features**: *`object`*

<a id="default_player_options.features.layout"></a>

###  layout

**● layout**: *`false`* = false

___
<a id="default_player_options.features.pip"></a>

###  pip

**● pip**: *`false`* = false

___
<a id="default_player_options.features.timecut"></a>

###  timeCut

**● timeCut**: *`false`* = false

___

___
<a id="default_player_options.html5"></a>

###  html5

**html5**: *`object`*

<a id="default_player_options.html5.hls"></a>

###  hls

**hls**: *`object`*

<a id="default_player_options.html5.hls.enablelowinitialplaylist"></a>

###  enableLowInitialPlaylist

**● enableLowInitialPlaylist**: *`false`* = false

___
<a id="default_player_options.html5.hls.overridenative"></a>

###  overrideNative

**● overrideNative**: *`true`* = true

___

___

___
<a id="default_player_options.youtube"></a>

###  youtube

**youtube**: *`object`*

<a id="default_player_options.youtube.disableblockerclick"></a>

###  disableBlockerClick

**● disableBlockerClick**: *`number`* = 1

___
<a id="default_player_options.youtube.modestbranding"></a>

###  modestbranding

**● modestbranding**: *`number`* = 1

___
<a id="default_player_options.youtube.customvars"></a>

###  customVars

**customVars**: *`object`*

<a id="default_player_options.youtube.customvars.origin"></a>

###  origin

**● origin**: *`string`* =  location.origin

___
<a id="default_player_options.youtube.customvars.playsinline-1"></a>

###  playsinline

**● playsinline**: *`number`* = 1

___
<a id="default_player_options.youtube.customvars.rel"></a>

###  rel

**● rel**: *`number`* = 0

___

___

___

___

