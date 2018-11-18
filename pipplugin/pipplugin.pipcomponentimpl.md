# PipComponentImpl

## Hierarchy

**PipComponentImpl**

## Implements

* [PipPlugin](pipplugin.pipplugin-1.md)

## Constructors

### constructor <a id="constructor"></a>

⊕ **new PipComponentImpl**\(player: `Player`, component: `Component`\): [PipComponentImpl](pipplugin.pipcomponentimpl.md)

**Parameters:**

| Name | Type |
| :--- | :--- |
| player | `Player` |
| component | `Component` |

**Returns:** [PipComponentImpl](pipplugin.pipcomponentimpl.md)

## Properties

### pipPlayer <a id="pipplayer"></a>

**● pipPlayer**: [_PlayerImplementation_](../annotoplayer/annotoplayer.playerimplementation.md)

## Methods

### disable <a id="disable"></a>

▸ **disable**\(\): `void`

**Returns:** `void`

### dispose <a id="dispose"></a>

▸ **dispose**\(\): `void`

**Returns:** `void`

### enable <a id="enable"></a>

▸ **enable**\(\): `void`

**Returns:** `void`

### hadnleTimeUpdateEvent <a id="hadnletimeupdateevent"></a>

▸ **hadnleTimeUpdateEvent**\(\): `void`

Throttled

**Returns:** `void`

### loadSrc <a id="loadsrc"></a>

▸ **loadSrc**\(src: [_SourceObject_](../annotoplayer/annotoplayer.sourceobject.md)\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| src | [SourceObject](../annotoplayer/annotoplayer.sourceobject.md) |

**Returns:** `void`

### ready <a id="ready"></a>

▸ **ready**\(\): `Promise`&lt;[PlayerImplementation](../annotoplayer/annotoplayer.playerimplementation.md)&gt;

**Returns:** `Promise`&lt;[PlayerImplementation](../annotoplayer/annotoplayer.playerimplementation.md)&gt;

### setAspectRatio <a id="setaspectratio"></a>

▸ **setAspectRatio**\(ratio: [_PlayerAspectRatio_](../annotoplayer/#playeraspectratio)\): `Promise`&lt;`any`&gt;

**Parameters:**

| Name | Type |
| :--- | :--- |
| ratio | [PlayerAspectRatio](../annotoplayer/#playeraspectratio) |

**Returns:** `Promise`&lt;`any`&gt;

### updateUI <a id="updateui"></a>

▸ **updateUI**\(ui: [_PipPluginUI_](pipplugin.pippluginui.md)\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| ui | [PipPluginUI](pipplugin.pippluginui.md) |

**Returns:** `void`

