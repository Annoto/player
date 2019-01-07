

# Hierarchy

**AnnotoPlayer**

# Constructors

<a id="constructor"></a>

##  constructor

⊕ **new AnnotoPlayer**(logger: *`LoggerInterface`*, widget: *`WidgetServiceInterface`*): [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

**Parameters:**

| Name | Type |
| ------ | ------ |
| logger | `LoggerInterface` |
| widget | `WidgetServiceInterface` |

**Returns:** [AnnotoPlayer](annotoplayer.annotoplayer-1.md)

___

# Accessors

<a id="aspectratio"></a>

##  aspectRatio

getaspectRatio(): [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)

**Returns:** [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)

___
<a id="currentsrc"></a>

##  currentSrc

getcurrentSrc(): [SourceObject](../interfaces/annotoplayer.sourceobject.md)

**Returns:** [SourceObject](../interfaces/annotoplayer.sourceobject.md)

___
<a id="currenttime"></a>

##  currentTime

getcurrentTime(): `number`

**Returns:** `number`

___
<a id="duration"></a>

##  duration

getduration(): `number`

**Returns:** `number`

___
<a id="fullscreen"></a>

##  fullscreen

getfullscreen(): `boolean`

**Returns:** `boolean`

___
<a id="issetup"></a>

##  isSetup

getisSetup(): `boolean`

**Returns:** `boolean`

___
<a id="paused"></a>

##  paused

getpaused(): `boolean`

**Returns:** `boolean`

___

# Methods

<a id="addtexttrack"></a>

##  addTextTrack

▸ **addTextTrack**(trackOpts: *[TextTrackOptions](../interfaces/annotoplayer.texttrackoptions.md)*):  `Promise`<`void`> &#124; `Promise`<`HTMLTrackElement`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| trackOpts | [TextTrackOptions](../interfaces/annotoplayer.texttrackoptions.md) |

**Returns:**  `Promise`<`void`> &#124; `Promise`<`HTMLTrackElement`>

___
<a id="close"></a>

##  close

▸ **close**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="closewidget"></a>

##  closeWidget

▸ **closeWidget**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="layout"></a>

##  layout

▸ **layout**(): `Promise`<[LayoutPlugin](../interfaces/layoutplugin.layoutplugin-1.md)>

**Returns:** `Promise`<[LayoutPlugin](../interfaces/layoutplugin.layoutplugin-1.md)>

___
<a id="loadsrc"></a>

##  loadSrc

▸ **loadSrc**(src?: *[SourceObject](../interfaces/annotoplayer.sourceobject.md)*, pipSrc?: *[SecondarySourceObject](../interfaces/annotoplayer.secondarysourceobject.md)*): `Promise`<[AnnotoPlayer](annotoplayer.annotoplayer-1.md)>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` src | [SourceObject](../interfaces/annotoplayer.sourceobject.md) |
| `Optional` pipSrc | [SecondarySourceObject](../interfaces/annotoplayer.secondarysourceobject.md) |

**Returns:** `Promise`<[AnnotoPlayer](annotoplayer.annotoplayer-1.md)>

___
<a id="loadwidget"></a>

##  loadWidget

▸ **loadWidget**(host?: *`HTMLElement`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`<`void`>

___
<a id="off"></a>

##  off

▸ **off**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="on"></a>

##  on

▸ **on**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="once"></a>

##  once

▸ **once**(eventT: *[PlayerEvent](../modules/annotoplayer.md#playerevent)*, cb: *[PlayerEventCallback](../modules/annotoplayer.md#playereventcallback)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| eventT | [PlayerEvent](../modules/annotoplayer.md#playerevent) |
| cb | [PlayerEventCallback](../modules/annotoplayer.md#playereventcallback) |

**Returns:** `Promise`<`void`>

___
<a id="pause"></a>

##  pause

▸ **pause**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="pip"></a>

##  pip

▸ **pip**(): `Promise`<[PipPlugin](../interfaces/pipplugin.pipplugin-1.md)>

**Returns:** `Promise`<[PipPlugin](../interfaces/pipplugin.pipplugin-1.md)>

___
<a id="play"></a>

##  play

▸ **play**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="removetexttrackkind"></a>

##  removeTextTrackKind

▸ **removeTextTrackKind**(kind: *[TextTrackKind](../modules/annotoplayer.md#texttrackkind)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| kind | [TextTrackKind](../modules/annotoplayer.md#texttrackkind) |

**Returns:** `Promise`<`void`>

___
<a id="reset"></a>

##  reset

▸ **reset**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="setaspectratio"></a>

##  setAspectRatio

▸ **setAspectRatio**(ratio: *[PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)*): `Promise`<`any`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| ratio | [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio) |

**Returns:** `Promise`<`any`>

___
<a id="setautoplay"></a>

##  setAutoplay

▸ **setAutoplay**(val: *`boolean`*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| val | `boolean` |

**Returns:** `void`

___
<a id="setpiplayout"></a>

##  setPipLayout

▸ **setPipLayout**(params: *[LayoutParams](../interfaces/layoutplugin.layoutparams.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| params | [LayoutParams](../interfaces/layoutplugin.layoutparams.md) |

**Returns:** `Promise`<`void`>

___
<a id="setpipui"></a>

##  setPipUI

▸ **setPipUI**(ui: *[PipPluginUI](../interfaces/pipplugin.pippluginui.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| ui | [PipPluginUI](../interfaces/pipplugin.pippluginui.md) |

**Returns:** `Promise`<`void`>

___
<a id="setposter"></a>

##  setPoster

▸ **setPoster**(posterUrl: *`string`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| posterUrl | `string` |

**Returns:** `Promise`<`void`>

___
<a id="setup"></a>

##  setup

▸ **setup**(element: * `string` &#124; `Element`*, options?: *[PlayerOptions](../interfaces/annotoplayer.playeroptions.md)*): `Promise`<`PlayerImplementation`>

**Parameters:**

| Name | Type | Default value |
| ------ | ------ | ------ |
| element |  `string` &#124; `Element`| - |
| `Default value` options | [PlayerOptions](../interfaces/annotoplayer.playeroptions.md) |  {} |

**Returns:** `Promise`<`PlayerImplementation`>

___
<a id="setupwidget"></a>

##  setupWidget

▸ **setupWidget**(options?: *`WidgetOptions`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` options | `WidgetOptions` |

**Returns:** `Promise`<`void`>

___
<a id="timecut"></a>

##  timeCut

▸ **timeCut**(): `Promise`<[TimeCutPlugin](../interfaces/timecutplugin.timecutplugin-1.md)>

**Returns:** `Promise`<[TimeCutPlugin](../interfaces/timecutplugin.timecutplugin-1.md)>

___

