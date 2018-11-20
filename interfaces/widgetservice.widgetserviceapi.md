

# Hierarchy

**WidgetServiceApi**

# Properties

<a id="setservices"></a>

##  setServices

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

# Methods

<a id="close"></a>

##  close

▸ **close**(): `Promise`<`void`>

**Returns:** `Promise`<`void`>

___
<a id="load"></a>

##  load

▸ **load**(playerElement: * `string` &#124; `HTMLElement`*, host?: *`HTMLElement`*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| playerElement |  `string` &#124; `HTMLElement`|
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`<`void`>

___
<a id="setup"></a>

##  setup

▸ **setup**(options?: *[WidgetOptions](annotoplayer.widgetoptions.md)*): `Promise`<`void`>

**Parameters:**

| Name | Type |
| ------ | ------ |
| `Optional` options | [WidgetOptions](annotoplayer.widgetoptions.md) |

**Returns:** `Promise`<`void`>

___

