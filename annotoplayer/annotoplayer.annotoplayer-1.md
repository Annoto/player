# AnnotoPlayer

## Hierarchy

**AnnotoPlayer**

## Constructors

### constructor <a id="constructor"></a>

⊕ **new AnnotoPlayer**\(assetLoader: [_AssetLoaderApi_](../services/services.assetloaderapi.md), logger: [_LoggerApi_](../services/services.loggerapi.md), authProvider?: [_AuthProviderApi_](annotoplayer.authproviderapi.md), deviceDetector?: `DeviceDetectorApi`, originProvider?: `OriginProvider`\): [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

**Parameters:**

| Name | Type |
| :--- | :--- |
| assetLoader | [AssetLoaderApi](../services/services.assetloaderapi.md) |
| logger | [LoggerApi](../services/services.loggerapi.md) |
| `Optional` authProvider | [AuthProviderApi](annotoplayer.authproviderapi.md) |
| `Optional` deviceDetector | `DeviceDetectorApi` |
| `Optional` originProvider | `OriginProvider` |

**Returns:** [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

## Accessors

### aspectRatio <a id="aspectratio"></a>

getaspectRatio\(\): [PlayerAspectRatio](./#playeraspectratio)

**Returns:** [PlayerAspectRatio](./#playeraspectratio)

### currentSrc <a id="currentsrc"></a>

getcurrentSrc\(\): [SourceObject](annotoplayer.sourceobject.md)

**Returns:** [SourceObject](annotoplayer.sourceobject.md)

### currentTime <a id="currenttime"></a>

getcurrentTime\(\): `number`

**Returns:** `number`

### duration <a id="duration"></a>

getduration\(\): `number`

**Returns:** `number`

### fullscreen <a id="fullscreen"></a>

getfullscreen\(\): `boolean`

**Returns:** `boolean`

### isSetup <a id="issetup"></a>

getisSetup\(\): `boolean`

**Returns:** `boolean`

### paused <a id="paused"></a>

getpaused\(\): `boolean`

**Returns:** `boolean`

## Methods

### addTextTrack <a id="addtexttrack"></a>

▸ **addTextTrack**\(trackOpts: [_TextTrackOptions_](annotoplayer.texttrackoptions.md)\): `Promise`&lt;`void`&gt; \| `Promise`&lt;`HTMLTrackElement`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| trackOpts | [TextTrackOptions](annotoplayer.texttrackoptions.md) |

**Returns:** `Promise`&lt;`void`&gt; \| `Promise`&lt;`HTMLTrackElement`&gt;

### close <a id="close"></a>

▸ **close**\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### closeWidget <a id="closewidget"></a>

▸ **closeWidget**\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### layout <a id="layout"></a>

▸ **layout**\(\): `Promise`&lt;[LayoutPlugin](../layoutplugin/layoutplugin.layoutplugin-1.md)&gt;

**Returns:** `Promise`&lt;[LayoutPlugin](../layoutplugin/layoutplugin.layoutplugin-1.md)&gt;

### loadSrc <a id="loadsrc"></a>

▸ **loadSrc**\(src?: [_SourceObject_](annotoplayer.sourceobject.md), pipSrc?: [_SecondarySourceObject_](annotoplayer.secondarysourceobject.md)\): `Promise`&lt;[AnnotoPlayer](annotoplayer.annotoplayer-1.md)&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` src | [SourceObject](annotoplayer.sourceobject.md) |
| `Optional` pipSrc | [SecondarySourceObject](annotoplayer.secondarysourceobject.md) |

**Returns:** `Promise`&lt;[AnnotoPlayer](annotoplayer.annotoplayer-1.md)&gt;

### loadWidget <a id="loadwidget"></a>

▸ **loadWidget**\(host?: `HTMLElement`\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`&lt;`void`&gt;

### off <a id="off"></a>

▸ **off**\(eventT: [_PlayerEvent_](./#playerevent), cb: [_PlayerEventCallback_](./#playereventcallback)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| eventT | [PlayerEvent](./#playerevent) |
| cb | [PlayerEventCallback](./#playereventcallback) |

**Returns:** `Promise`&lt;`void`&gt;

### on <a id="on"></a>

▸ **on**\(eventT: [_PlayerEvent_](./#playerevent), cb: [_PlayerEventCallback_](./#playereventcallback)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| eventT | [PlayerEvent](./#playerevent) |
| cb | [PlayerEventCallback](./#playereventcallback) |

**Returns:** `Promise`&lt;`void`&gt;

### once <a id="once"></a>

▸ **once**\(eventT: [_PlayerEvent_](./#playerevent), cb: [_PlayerEventCallback_](./#playereventcallback)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| eventT | [PlayerEvent](./#playerevent) |
| cb | [PlayerEventCallback](./#playereventcallback) |

**Returns:** `Promise`&lt;`void`&gt;

### pause <a id="pause"></a>

▸ **pause**\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### pip <a id="pip"></a>

▸ **pip**\(\): `Promise`&lt;[PipPlugin](../pipplugin/pipplugin.pipplugin-1.md)&gt;

**Returns:** `Promise`&lt;[PipPlugin](../pipplugin/pipplugin.pipplugin-1.md)&gt;

### play <a id="play"></a>

▸ **play**\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### removeTextTrackKind <a id="removetexttrackkind"></a>

▸ **removeTextTrackKind**\(kind: [_TextTrackKind_](./#texttrackkind)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| kind | [TextTrackKind](./#texttrackkind) |

**Returns:** `Promise`&lt;`void`&gt;

### reset <a id="reset"></a>

▸ **reset**\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### setAspectRatio <a id="setaspectratio"></a>

▸ **setAspectRatio**\(ratio: [_PlayerAspectRatio_](./#playeraspectratio)\): `Promise`&lt;`any`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| ratio | [PlayerAspectRatio](./#playeraspectratio) |

**Returns:** `Promise`&lt;`any`&gt;

### setAutoplay <a id="setautoplay"></a>

▸ **setAutoplay**\(val: `boolean`\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| val | `boolean` |

**Returns:** `void`

### setPipLayout <a id="setpiplayout"></a>

▸ **setPipLayout**\(params: [_LayoutParams_](../layoutplugin/layoutplugin.layoutparams.md)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| params | [LayoutParams](../layoutplugin/layoutplugin.layoutparams.md) |

**Returns:** `Promise`&lt;`void`&gt;

### setPipUI <a id="setpipui"></a>

▸ **setPipUI**\(ui: [_PipPluginUI_](../pipplugin/pipplugin.pippluginui.md)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| ui | [PipPluginUI](../pipplugin/pipplugin.pippluginui.md) |

**Returns:** `Promise`&lt;`void`&gt;

### setPoster <a id="setposter"></a>

▸ **setPoster**\(posterUrl: `string`\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| posterUrl | `string` |

**Returns:** `Promise`&lt;`void`&gt;

### setup <a id="setup"></a>

▸ **setup**\(element:  __`string` _\|_ `Element`, options?: [_PlayerOptions_](annotoplayer.playeroptions.md)\): `Promise`&lt;[PlayerImplementation](annotoplayer.playerimplementation.md)&gt;

**Parameters:**

| Name | Type | Default value |
| :--- | :--- | :--- |
| element | `string` \| `Element` | - |
| `Default value` options | [PlayerOptions](annotoplayer.playeroptions.md) | {} |

**Returns:** `Promise`&lt;[PlayerImplementation](annotoplayer.playerimplementation.md)&gt;

### setupWidget <a id="setupwidget"></a>

▸ **setupWidget**\(options?: [_WidgetOptions_](annotoplayer.widgetoptions.md)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` options | [WidgetOptions](annotoplayer.widgetoptions.md) |

**Returns:** `Promise`&lt;`void`&gt;

### timeCut <a id="timecut"></a>

▸ **timeCut**\(\): `Promise`&lt;[TimeCutPlugin](../timecutplugin/timecutplugin.timecutplugin-1.md)&gt;

**Returns:** `Promise`&lt;[TimeCutPlugin](../timecutplugin/timecutplugin.timecutplugin-1.md)&gt;

