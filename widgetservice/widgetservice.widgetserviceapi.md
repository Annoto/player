# WidgetServiceApi

## Hierarchy

**WidgetServiceApi**

## Properties

### close <a id="close"></a>

**● close**: `function`

#### Type declaration

▸\(\): `Promise`&lt;`void`&gt;

**Returns:** `Promise`&lt;`void`&gt;

### load <a id="load"></a>

**● load**: `function`

#### Type declaration

▸\(playerElement:  __`string` _\|_ `HTMLElement`, host?: `HTMLElement`\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| playerElement | `string` \| `HTMLElement` |
| `Optional` host | `HTMLElement` |

**Returns:** `Promise`&lt;`void`&gt;

### setServices <a id="setservices"></a>

**● setServices**: `function`

#### Type declaration

▸\(assetLoader: [_AssetLoaderApi_](../services/services.assetloaderapi.md), logger: [_LoggerApi_](../services/services.loggerapi.md), authProvider?: [_AuthProviderApi_](../annotoplayer/annotoplayer.authproviderapi.md), deviceDetector?: `DeviceDetectorApi`, originProvider?: `OriginProvider`\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| assetLoader | [AssetLoaderApi](../services/services.assetloaderapi.md) |
| logger | [LoggerApi](../services/services.loggerapi.md) |
| `Optional` authProvider | [AuthProviderApi](../annotoplayer/annotoplayer.authproviderapi.md) |
| `Optional` deviceDetector | `DeviceDetectorApi` |
| `Optional` originProvider | `OriginProvider` |

**Returns:** `void`

### setup <a id="setup"></a>

**● setup**: `function`

#### Type declaration

▸\(options?: [_WidgetOptions_](../annotoplayer/annotoplayer.widgetoptions.md)\): `Promise`&lt;`void`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` options | [WidgetOptions](../annotoplayer/annotoplayer.widgetoptions.md) |

**Returns:** `Promise`&lt;`void`&gt;

