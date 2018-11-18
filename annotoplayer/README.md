# annotoPlayer

## Index

#### Classes

* [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

#### Interfaces

* [AuthProviderApi](annotoplayer.authproviderapi.md)
* [PlayerImplementation](annotoplayer.playerimplementation.md)
* [PlayerOptions](annotoplayer.playeroptions.md)
* [PlayerServices](annotoplayer.playerservices.md)
* [SecondarySourceObject](annotoplayer.secondarysourceobject.md)
* [SourceObject](annotoplayer.sourceobject.md)
* [TextTrackOptions](annotoplayer.texttrackoptions.md)
* [WidgetOptions](annotoplayer.widgetoptions.md)
* [WidgetUxOptions](annotoplayer.widgetuxoptions.md)

#### Type aliases

* [PlayerAspectRatio](./#playeraspectratio)
* [PlayerEvent](./#playerevent)
* [PlayerEventCallback](./#playereventcallback)
* [TextTrackKind](./#texttrackkind)
* [TextTrackMode](./#texttrackmode)
* [VideoType](./#videotype)

#### Functions

* [annotoPlayer](./#annotoplayer-2)

#### Object literals

* [DEFAULT\_PLAYER\_OPTIONS](./#default_player_options)

## Type aliases

### PlayerAspectRatio <a id="playeraspectratio"></a>

**Ƭ PlayerAspectRatio**:  _"239:100" \| "16:9" \| "16:10" \| "4:3" \| "100:239" \| "9:16" \| "10:16" \| "3:4" \| "auto"_ 

### PlayerEvent <a id="playerevent"></a>

**Ƭ PlayerEvent**:  _"play" \| "pause" \| "seeked" \| "seeking" \| "timeupdate" \| "fullscreenchange" \| "ratechange" \| "volumechange" \| "loadedmetadata" \| "durationchange" \| "progress" \| "waiting" \| "playing" \| "loadstart"_ 

### PlayerEventCallback <a id="playereventcallback"></a>

**Ƭ PlayerEventCallback**: `function`

**Type declaration**

▸\(arg?: `any`\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` arg | `any` |

**Returns:** `void`

### TextTrackKind <a id="texttrackkind"></a>

**Ƭ TextTrackKind**: `Videojs.TextTrack.Kind`

### TextTrackMode <a id="texttrackmode"></a>

**Ƭ TextTrackMode**: `Videojs.TextTrack.Mode`

### VideoType <a id="videotype"></a>

**Ƭ VideoType**:  _"video/mp4" \| "video/webm" \| "video/youtube" \| "application/x-mpegURL"_ 

## Functions

### annotoPlayer <a id="annotoplayer-2"></a>

▸ **annotoPlayer**\(elementOrId:  __`string` _\|_ `HTMLElement`, options?: [_PlayerOptions_](annotoplayer.playeroptions.md), services?: [_PlayerServices_](annotoplayer.playerservices.md)\): `Promise`&lt;[AnnotoPlayer](annotoplayer.annotoplayer-1.md)&gt;

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| elementOrId | `string` \| `HTMLElement` | Id of HTMLElement or the element DOM element |
| `Optional` options | [PlayerOptions](annotoplayer.playeroptions.md) | player options |
| `Optional` services | [PlayerServices](annotoplayer.playerservices.md) | player services |

**Returns:** `Promise`&lt;[AnnotoPlayer](annotoplayer.annotoplayer-1.md)&gt; Promise that resolves with the player instance

## Object literals

### `<Const>` DEFAULT\_PLAYER\_OPTIONS <a id="default_player_options"></a>

**DEFAULT\_PLAYER\_OPTIONS**: `object`

#### controls <a id="default_player_options.controls"></a>

**● controls**: `true` = true

#### defaultVolume <a id="default_player_options.defaultvolume"></a>

**● defaultVolume**: `number` = 0.5

#### playbackRates <a id="default_player_options.playbackrates"></a>

**● playbackRates**: `number`_\[\]_ = \[0.75, 1, 1.25, 1.5, 1.75, 2\]

#### playsinline <a id="default_player_options.playsinline"></a>

**● playsinline**: `true` = true

#### preload <a id="default_player_options.preload"></a>

**● preload**: `string` = "auto"

#### sources <a id="default_player_options.sources"></a>

**● sources**: `undefined`_\[\]_ = \[\]

#### techOrder <a id="default_player_options.techorder"></a>

**● techOrder**: `string`_\[\]_ = \['html5', 'youtube'\]

#### features <a id="default_player_options.features"></a>

**features**: `object`

#### layout <a id="default_player_options.features.layout"></a>

**● layout**: `false` = false

#### pip <a id="default_player_options.features.pip"></a>

**● pip**: `false` = false

#### timeCut <a id="default_player_options.features.timecut"></a>

**● timeCut**: `false` = false

#### html5 <a id="default_player_options.html5"></a>

**html5**: `object`

#### hls <a id="default_player_options.html5.hls"></a>

**hls**: `object`

#### enableLowInitialPlaylist <a id="default_player_options.html5.hls.enablelowinitialplaylist"></a>

**● enableLowInitialPlaylist**: `false` = false

#### overrideNative <a id="default_player_options.html5.hls.overridenative"></a>

**● overrideNative**: `true` = true

#### youtube <a id="default_player_options.youtube"></a>

**youtube**: `object`

#### disableBlockerClick <a id="default_player_options.youtube.disableblockerclick"></a>

**● disableBlockerClick**: `number` = 1

#### modestbranding <a id="default_player_options.youtube.modestbranding"></a>

**● modestbranding**: `number` = 1

#### customVars <a id="default_player_options.youtube.customvars"></a>

**customVars**: `object`

#### origin <a id="default_player_options.youtube.customvars.origin"></a>

**● origin**: `string` = location.origin

#### playsinline <a id="default_player_options.youtube.customvars.playsinline-1"></a>

**● playsinline**: `number` = 1

#### rel <a id="default_player_options.youtube.customvars.rel"></a>

**● rel**: `number` = 0

