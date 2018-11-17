[Annoto Player](../README.md) > [pipPlugin](../modules/pipplugin.md) > [PipComponentImpl](../classes/pipplugin.pipcomponentimpl.md)

# Class: PipComponentImpl

## Hierarchy

**PipComponentImpl**

## Implements

* [PipPlugin](../interfaces/pipplugin.pipplugin-1.md)

## Index

### Constructors

* [constructor](pipplugin.pipcomponentimpl.md#constructor)

### Properties

* [pipPlayer](pipplugin.pipcomponentimpl.md#pipplayer)

### Methods

* [disable](pipplugin.pipcomponentimpl.md#disable)
* [dispose](pipplugin.pipcomponentimpl.md#dispose)
* [enable](pipplugin.pipcomponentimpl.md#enable)
* [hadnleTimeUpdateEvent](pipplugin.pipcomponentimpl.md#hadnletimeupdateevent)
* [loadSrc](pipplugin.pipcomponentimpl.md#loadsrc)
* [ready](pipplugin.pipcomponentimpl.md#ready)
* [setAspectRatio](pipplugin.pipcomponentimpl.md#setaspectratio)
* [updateUI](pipplugin.pipcomponentimpl.md#updateui)

---

## Constructors

<a id="constructor"></a>

###  constructor

⊕ **new PipComponentImpl**(player: *`Player`*, component: *`Component`*): [PipComponentImpl](pipplugin.pipcomponentimpl.md)

**Parameters:**

| Name | Type |
| ------ | ------ |
| player | `Player` |
| component | `Component` |

**Returns:** [PipComponentImpl](pipplugin.pipcomponentimpl.md)

___

## Properties

<a id="pipplayer"></a>

###  pipPlayer

**● pipPlayer**: *[PlayerImplementation](../interfaces/annotoplayer.playerimplementation.md)*

___

## Methods

<a id="disable"></a>

###  disable

▸ **disable**(): `void`

**Returns:** `void`

___
<a id="dispose"></a>

###  dispose

▸ **dispose**(): `void`

**Returns:** `void`

___
<a id="enable"></a>

###  enable

▸ **enable**(): `void`

**Returns:** `void`

___
<a id="hadnletimeupdateevent"></a>

###  hadnleTimeUpdateEvent

▸ **hadnleTimeUpdateEvent**(): `void`

Throttled

**Returns:** `void`

___
<a id="loadsrc"></a>

###  loadSrc

▸ **loadSrc**(src: *[SourceObject](../interfaces/annotoplayer.sourceobject.md)*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| src | [SourceObject](../interfaces/annotoplayer.sourceobject.md) |

**Returns:** `void`

___
<a id="ready"></a>

###  ready

▸ **ready**(): `Promise`<[PlayerImplementation](../interfaces/annotoplayer.playerimplementation.md)>

**Returns:** `Promise`<[PlayerImplementation](../interfaces/annotoplayer.playerimplementation.md)>

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
<a id="updateui"></a>

###  updateUI

▸ **updateUI**(ui: *[PipPluginUI](../interfaces/pipplugin.pippluginui.md)*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| ui | [PipPluginUI](../interfaces/pipplugin.pippluginui.md) |

**Returns:** `void`

___

