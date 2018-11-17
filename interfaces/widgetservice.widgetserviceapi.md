[Annoto Player](../README.md) > [widgetService](../modules/widgetservice.md) > [WidgetServiceApi](../interfaces/widgetservice.widgetserviceapi.md)

# Interface: WidgetServiceApi

## Hierarchy

**WidgetServiceApi**

## Index

### Properties

* [close](widgetservice.widgetserviceapi.md#close)
* [load](widgetservice.widgetserviceapi.md#load)
* [setServices](widgetservice.widgetserviceapi.md#setservices)
* [setup](widgetservice.widgetserviceapi.md#setup)

---

## Properties

<a id="close"></a>

###  close

**● close**: *`function`*

#### Type declaration
▸(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="load"></a>

###  load

**● load**: *`function`*

#### Type declaration
▸(playerElement: * `string` &#124; `HTMLElement`*, host?: *`HTMLElement`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| playerElement |  `string` &#124; `HTMLElement`|
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`<`void`>

___
<a id="setservices"></a>

###  setServices

**● setServices**: *`function`*

#### Type declaration
▸(assetLoader: *[AssetLoaderApi](services.assetloaderapi.md)*, logger: *[LoggerApi](services.loggerapi.md)*, authProvider?: *[AuthProviderApi](annotoplayer.authproviderapi.md)*, deviceDetector?: *`DeviceDetectorApi`*, originProvider?: *`OriginProvider`*): `void`

**Parameters:**

| Name | Type |
| ------ | ------ |
| assetLoader | [AssetLoaderApi](services.assetloaderapi.md) |
| logger | [LoggerApi](services.loggerapi.md) |
| `Optional` authProvider | [AuthProviderApi](annotoplayer.authproviderapi.md) |
| `Optional` deviceDetector | `DeviceDetectorApi` |
| `Optional` originProvider | `OriginProvider` |

**Returns:** `void`

___
<a id="setup"></a>

###  setup

**● setup**: *`function`*

#### Type declaration
▸(options?: *[WidgetOptions](annotoplayer.widgetoptions.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` options | [WidgetOptions](annotoplayer.widgetoptions.md) |

**Returns:** `Promise`<`void`>

___

