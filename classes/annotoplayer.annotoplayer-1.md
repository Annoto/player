[Annoto Player](../README.md) > [annotoPlayer](../modules/annotoplayer.md) > [AnnotoPlayer](../classes/annotoplayer.annotoplayer-1.md)

# Class: AnnotoPlayer

## Hierarchy

**AnnotoPlayer**

## Index

### Constructors

* [constructor](annotoplayer.annotoplayer-1.md#constructor)

### Accessors

* [aspectRatio](annotoplayer.annotoplayer-1.md#aspectratio)
* [currentSrc](annotoplayer.annotoplayer-1.md#currentsrc)
* [currentTime](annotoplayer.annotoplayer-1.md#currenttime)
* [duration](annotoplayer.annotoplayer-1.md#duration)
* [fullscreen](annotoplayer.annotoplayer-1.md#fullscreen)
* [isSetup](annotoplayer.annotoplayer-1.md#issetup)
* [paused](annotoplayer.annotoplayer-1.md#paused)

### Methods

* [addTextTrack](annotoplayer.annotoplayer-1.md#addtexttrack)
* [close](annotoplayer.annotoplayer-1.md#close)
* [closeWidget](annotoplayer.annotoplayer-1.md#closewidget)
* [layout](annotoplayer.annotoplayer-1.md#layout)
* [loadSrc](annotoplayer.annotoplayer-1.md#loadsrc)
* [loadWidget](annotoplayer.annotoplayer-1.md#loadwidget)
* [off](annotoplayer.annotoplayer-1.md#off)
* [on](annotoplayer.annotoplayer-1.md#on)
* [once](annotoplayer.annotoplayer-1.md#once)
* [pause](annotoplayer.annotoplayer-1.md#pause)
* [pip](annotoplayer.annotoplayer-1.md#pip)
* [play](annotoplayer.annotoplayer-1.md#play)
* [removeTextTrackKind](annotoplayer.annotoplayer-1.md#removetexttrackkind)
* [reset](annotoplayer.annotoplayer-1.md#reset)
* [setAspectRatio](annotoplayer.annotoplayer-1.md#setaspectratio)
* [setAutoplay](annotoplayer.annotoplayer-1.md#setautoplay)
* [setPipLayout](annotoplayer.annotoplayer-1.md#setpiplayout)
* [setPipUI](annotoplayer.annotoplayer-1.md#setpipui)
* [setPoster](annotoplayer.annotoplayer-1.md#setposter)
* [setup](annotoplayer.annotoplayer-1.md#setup)
* [setupWidget](annotoplayer.annotoplayer-1.md#setupwidget)
* [timeCut](annotoplayer.annotoplayer-1.md#timecut)

---

## Constructors

<a id="constructor"></a>

###  constructor

⊕ **new AnnotoPlayer**(assetLoader: *[AssetLoaderApi](../interfaces/services.assetloaderapi.md)*, logger: *[LoggerApi](../interfaces/services.loggerapi.md)*, authProvider?: *[AuthProviderApi](../interfaces/annotoplayer.authproviderapi.md)*, deviceDetector?: *`DeviceDetectorApi`*, originProvider?: *`OriginProvider`*): [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

**Parameters:**

| Name | Type |
| ------ | ------ |
| assetLoader | [AssetLoaderApi](../interfaces/services.assetloaderapi.md) |
| logger | [LoggerApi](../interfaces/services.loggerapi.md) |
| `Optional` authProvider | [AuthProviderApi](../interfaces/annotoplayer.authproviderapi.md) |
| `Optional` deviceDetector | `DeviceDetectorApi` |
| `Optional` originProvider | `OriginProvider` |

**Returns:** [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

___

## Accessors

<a id="aspectratio"></a>

###  aspectRatio

getaspectRatio(): [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)

**Returns:** [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)

___
<a id="currentsrc"></a>

###  currentSrc

getcurrentSrc(): [SourceObject](../interfaces/annotoplayer.sourceobject.md)

**Returns:** [SourceObject](../interfaces/annotoplayer.sourceobject.md)

___
<a id="currenttime"></a>

###  currentTime

getcurrentTime(): `number`

**Returns:** `number`

___
<a id="duration"></a>

###  duration

getduration(): `number`

**Returns:** `number`

___
<a id="fullscreen"></a>

###  fullscreen

getfullscreen(): `boolean`

**Returns:** `boolean`

___
<a id="issetup"></a>

###  isSetup

getisSetup(): `boolean`

**Returns:** `boolean`

___
<a id="paused"></a>

###  paused

getpaused(): `boolean`

**Returns:** `boolean`

___

## Methods

<a id="addtexttrack"></a>

###  addTextTrack

▸ **addTextTrack**(trackOpts: *[TextTrackOptions](../interfaces/annotoplayer.texttrackoptions.md)*):  `Promise`<`void`> &#124; `Promise`<`HTMLTrackElement`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| trackOpts | [TextTrackOptions](../interfaces/annotoplayer.texttrackoptions.md) |

**Returns:**  `Promise`<`void`> &#124; `Promise`<`HTMLTrackElement`>

___
<a id="close"></a>

###  close

▸ **close**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="closewidget"></a>

###  closeWidget

▸ **closeWidget**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="layout"></a>

###  layout

▸ **layout**(): `Promise`<[LayoutPlugin](../interfaces/layoutplugin.layoutplugin-1.md)>

**Returns:** `Promise`<[LayoutPlugin](../interfaces/layoutplugin.layoutplugin-1.md)>

___
<a id="loadsrc"></a>

###  loadSrc

▸ **loadSrc**(src?: *[SourceObject](../interfaces/annotoplayer.sourceobject.md)*, pipSrc?: *[SecondarySourceObject](../interfaces/annotoplayer.secondarysourceobject.md)*): `Promise`<[AnnotoPlayer](annotoplayer.annotoplayer-1.md)>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` src | [SourceObject](../interfaces/annotoplayer.sourceobject.md) |
| `Optional` pipSrc | [SecondarySourceObject](../interfaces/annotoplayer.secondarysourceobject.md) |

**Returns:** `Promise`<[AnnotoPlayer](annotoplayer.annotoplayer-1.md)>

___
<a id="loadwidget"></a>

###  loadWidget

▸ **loadWidget**(host?: *`HTMLElement`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`<`void`>

___
<a id="off"></a>

###  off

▸ **off**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="on"></a>

###  on

▸ **on**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="once"></a>

###  once

▸ **once**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="pause"></a>

###  pause

▸ **pause**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="pip"></a>

###  pip

▸ **pip**(): `Promise`<[PipPlugin](../interfaces/pipplugin.pipplugin-1.md)>

**Returns:** `Promise`<[PipPlugin](../interfaces/pipplugin.pipplugin-1.md)>

___
<a id="play"></a>

###  play

▸ **play**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="removetexttrackkind"></a>

###  removeTextTrackKind

▸ **removeTextTrackKind**(kind: *[TextTrackKind](../modules/annotoplayer.md#texttrackkind)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| kind | [TextTrackKind](../modules/annotoplayer.md#texttrackkind) |

**Returns:** `Promise`<`void`>

___
<a id="reset"></a>

###  reset

▸ **reset**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="setaspectratio"></a>

###  setAspectRatio

▸ **setAspectRatio**(ratio: *[PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)*): `Promise`<`any`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| ratio | [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio) |

**Returns:** `Promise`<`any`>

___
<a id="setautoplay"></a>

###  setAutoplay

▸ **setAutoplay**(val: *`boolean`*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| val | `boolean` |

**Returns:** `void`

___
<a id="setpiplayout"></a>

###  setPipLayout

▸ **setPipLayout**(params: *[LayoutParams](../interfaces/layoutplugin.layoutparams.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| params | [LayoutParams](../interfaces/layoutplugin.layoutparams.md) |

**Returns:** `Promise`<`void`>

___
<a id="setpipui"></a>

###  setPipUI

▸ **setPipUI**(ui: *[PipPluginUI](../interfaces/pipplugin.pippluginui.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| ui | [PipPluginUI](../interfaces/pipplugin.pippluginui.md) |

**Returns:** `Promise`<`void`>

___
<a id="setposter"></a>

###  setPoster

▸ **setPoster**(posterUrl: *`string`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| posterUrl | `string` |

**Returns:** `Promise`<`void`>

___
<a id="setup"></a>

###  setup

▸ **setup**(element: * `string` &#124; `Element`*, options?: *[PlayerOptions](../interfaces/annotoplayer.playeroptions.md)*): `Promise`<[PlayerImplementation](../interfaces/annotoplayer.playerimplementation.md)>

**Parameters:**

| Name | Type | Default value |
| ------ | ------ | ------ |
| element |  `string` &#124; `Element`| - |
| `Default value` options | [PlayerOptions](../interfaces/annotoplayer.playeroptions.md) |  {} |

**Returns:** `Promise`<[PlayerImplementation](../interfaces/annotoplayer.playerimplementation.md)>

___
<a id="setupwidget"></a>

###  setupWidget

▸ **setupWidget**(options?: *[WidgetOptions](../interfaces/annotoplayer.widgetoptions.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` options | [WidgetOptions](../interfaces/annotoplayer.widgetoptions.md) |

**Returns:** `Promise`<`void`>

___
<a id="timecut"></a>

###  timeCut

▸ **timeCut**(): `Promise`<[TimeCutPlugin](../interfaces/timecutplugin.timecutplugin-1.md)>

**Returns:** `Promise`<[TimeCutPlugin](../interfaces/timecutplugin.timecutplugin-1.md)>

___

