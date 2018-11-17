[Annoto Player](../README.md) > [pipPlugin](../modules/pipplugin.md) > [PipPlugin](../interfaces/pipplugin.pipplugin-1.md)

# Interface: PipPlugin

## Hierarchy

**PipPlugin**

## Implemented by

* [PipComponentImpl](../classes/pipplugin.pipcomponentimpl.md)

## Index

### Properties

* [disable](pipplugin.pipplugin-1.md#disable)
* [dispose](pipplugin.pipplugin-1.md#dispose)
* [enable](pipplugin.pipplugin-1.md#enable)
* [loadSrc](pipplugin.pipplugin-1.md#loadsrc)
* [ready](pipplugin.pipplugin-1.md#ready)
* [setAspectRatio](pipplugin.pipplugin-1.md#setaspectratio)
* [updateUI](pipplugin.pipplugin-1.md#updateui)

---

## Properties

<a id="disable"></a>

###  disable

**● disable**: *`function`*

#### Type declaration
▸(): `void`

**Returns:** `void`

___
<a id="dispose"></a>

###  dispose

**● dispose**: *`function`*

#### Type declaration
▸(): `void`

**Returns:** `void`

___
<a id="enable"></a>

###  enable

**● enable**: *`function`*

#### Type declaration
▸(): `void`

**Returns:** `void`

___
<a id="loadsrc"></a>

###  loadSrc

**● loadSrc**: *`function`*

#### Type declaration
▸(src: *[SourceObject](annotoplayer.sourceobject.md)*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| src | [SourceObject](annotoplayer.sourceobject.md) |

**Returns:** `void`

___
<a id="ready"></a>

###  ready

**● ready**: *`function`*

#### Type declaration
▸(): `Promise`<[PlayerImplementation](annotoplayer.playerimplementation.md)>

**Returns:** `Promise`<[PlayerImplementation](annotoplayer.playerimplementation.md)>

___
<a id="setaspectratio"></a>

###  setAspectRatio

**● setAspectRatio**: *`function`*

#### Type declaration
▸(ratio: *[PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio)*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| ratio | [PlayerAspectRatio](../modules/annotoplayer.md#playeraspectratio) |

**Returns:** `void`

___
<a id="updateui"></a>

###  updateUI

**● updateUI**: *`function`*

#### Type declaration
▸(ui: *[PipPluginUI](pipplugin.pippluginui.md)*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| ui | [PipPluginUI](pipplugin.pippluginui.md) |

**Returns:** `void`

___

