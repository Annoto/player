# PlayerImplementation

## Hierarchy

`Player`

**↳ PlayerImplementation**

## Properties

### Player <a id="player"></a>

**● Player**: `object`

#### Type declaration

### bigPlayButton <a id="bigplaybutton"></a>

**● bigPlayButton**: `Button`

### children\_ <a id="children_"></a>

**● children\_**: `Component`_\[\]_

### controlBar <a id="controlbar"></a>

**● controlBar**: `ControlBar`

### errorDisplay <a id="errordisplay"></a>

**● errorDisplay**: `ModalDialog`

### layout <a id="layout"></a>

**● layout**: `function`

#### Type declaration

▸\(options?: [_LayoutPluginOptions_](../layoutplugin/layoutplugin.layoutpluginoptions.md)\): [LayoutPlugin](../layoutplugin/layoutplugin.layoutplugin-1.md)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` options | [LayoutPluginOptions](../layoutplugin/layoutplugin.layoutpluginoptions.md) |

**Returns:** [LayoutPlugin](../layoutplugin/layoutplugin.layoutplugin-1.md)

### loadingSpinner <a id="loadingspinner"></a>

**● loadingSpinner**: `Component`

### options\_ <a id="options_"></a>

**● options\_**: `PlayerOptions`

### pip <a id="pip"></a>

**● pip**: `function`

#### Type declaration

▸\(options?: [_PipPluginOptions_](../pipplugin/pipplugin.pippluginoptions.md)\): [PipPlugin](../pipplugin/pipplugin.pipplugin-1.md)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` options | [PipPluginOptions](../pipplugin/pipplugin.pippluginoptions.md) |

**Returns:** [PipPlugin](../pipplugin/pipplugin.pipplugin-1.md)

### player\_ <a id="player_"></a>

**● player\_**: `Player`

### timeCut <a id="timecut"></a>

**● timeCut**: `function`

#### Type declaration

▸\(option?: [_TimeCutPluginOptions_](../timecutplugin/timecutplugin.timecutpluginoptions.md)\): [TimeCutPlugin](../timecutplugin/timecutplugin.timecutplugin-1.md)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` option | [TimeCutPluginOptions](../timecutplugin/timecutplugin.timecutpluginoptions.md) |

**Returns:** [TimeCutPlugin](../timecutplugin/timecutplugin.timecutplugin-1.md)

### userActive\_ <a id="useractive_"></a>

**● userActive\_**: `boolean`

### userActivity\_ <a id="useractivity_"></a>

**● userActivity\_**: `boolean`

## Methods

### $ <a id="_"></a>

▸ **$**\(selector: `string`, context?:  __`string` _\|_ `Element`\): `Element`

Find a single DOM element matching a `selector`. This can be within the `Component`s `contentEl()` or another custom context. _**see**_: [Information on CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_Started/Selectors)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| selector | `string` | `A valid CSS selector, which will be passed to &#x60;querySelector&#x60;.` |
| `Optional` context | `string` \| `Element` |  |

**Returns:** `Element` the dom element that was found, or null

### $$ <a id="__"></a>

▸ **$$**\(selector: `string`, context?:  __`string` _\|_ `Element`\): `NodeList`

Finds all DOM element matching a `selector`. This can be within the `Component`s `contentEl()` or another custom context. _**see**_: [Information on CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_Started/Selectors)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| selector | `string` | `A valid CSS selector, which will be passed to &#x60;querySelectorAll&#x60;.` |
| `Optional` context | `string` \| `Element` |  |

**Returns:** `NodeList` a list of dom elements that were found

### addChild <a id="addchild"></a>

▸ **addChild**\(component: `string`, optionsopt?: `any`, indexopt?: `number`\): `Component`

▸ **addChild**\(component: `Element`, optionsopt?: `any`, indexopt?: `number`\): `Element`

▸ **addChild**&lt;`T`&gt;\(child:  __`string` _\|_ `T`, options?: `any`, index?: `number`\): `T`

Add a child `Component` inside the current `Component`.

**Parameters:**

| Name | Type |
| :--- | :--- |
| component | `string` |
| `Optional` optionsopt | `any` |
| `Optional` indexopt | `number` |

**Returns:** `Component` The `Component` that gets added as a child. When using a string the `Component` will get created by this process.

**Parameters:**

| Name | Type |
| :--- | :--- |
| component | `Element` |
| `Optional` optionsopt | `any` |
| `Optional` indexopt | `number` |

**Returns:** `Element`

**Type parameters:**

#### T :  `Component`

**Parameters:**

| Name | Type |
| :--- | :--- |
| child | `string` \| `T` |
| `Optional` options | `any` |
| `Optional` index | `number` |

**Returns:** `T`

### addClass <a id="addclass"></a>

▸ **addClass**\(classToAdd: `string`\): `void`

Add a CSS class name to the `Component`s element.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| classToAdd | `string` | `CSS class name to add` |

**Returns:** `void`

### addRemoteTextTrack <a id="addremotetexttrack"></a>

▸ **addRemoteTextTrack**\(options: `TextTrackOptions`, manualCleanup: `boolean`\): `HTMLTrackElement`

Create a remote {@link TextTrack} and an {@link HTMLTrackElement}. It will automatically removed from the video element whenever the source changes, unless manualCleanup is set to false.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| options | `TextTrackOptions` | `Options to pass to {@link HTMLTrackElement} during creation. See{@link HTMLTrackElement} for object properties that you should use.` |
| manualCleanup | `boolean` |  |

**Returns:** `HTMLTrackElement` the HTMLTrackElement that was created and added to the HtmlTrackElementList and the remote TextTrackList

### addTextTrack <a id="addtexttrack"></a>

▸ **addTextTrack**\(kind?: `string`, label?: `string`, language?: `string`\): `void`

A helper method for adding a {@link TextTrack} to our {@link TextTrackList}.

In addition to the W3C settings we allow adding additional info through options. _**see**_: [http://www.w3.org/html/wg/drafts/html/master/embedded-content-0.html\#dom-media-addtexttrack](http://www.w3.org/html/wg/drafts/html/master/embedded-content-0.html#dom-media-addtexttrack)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` kind | `string` |
| `Optional` label | `string` |
| `Optional` language | `string` |

**Returns:** `void` the TextTrack that was added or undefined if there is no tech

### aspectRatio <a id="aspectratio"></a>

▸ **aspectRatio**\(ratio: `string`\): `void`

▸ **aspectRatio**\(\): `string`

A getter/setter for the `Player`'s aspect ratio.

**Parameters:**

| Name | Type |
| :--- | :--- |
| ratio | `string` |

**Returns:** `void`

* The current aspect ratio of the `Player` when getting.
  * undefined when setting

**Returns:** `string`

### autoplay <a id="autoplay"></a>

▸ **autoplay**\(value?:  __`boolean` _\|_ `string`\): `void`

▸ **autoplay**\(\): `boolean` \| `string`

Get or set the autoplay option. When this is a boolean it will modify the attribute on the tech. When this is a string the attribute on the tech will be removed and `Player` will handle autoplay on loadstarts.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` value | `boolean` \| `string` |

**Returns:** `void` The current value of autoplay when getting

**Returns:** `boolean` \| `string`

### blur <a id="blur"></a>

▸ **blur**\(\): `void`

Remove the focus from this component

**Returns:** `void`

### buffered <a id="buffered"></a>

▸ **buffered**\(\): `TimeRange`

Get a TimeRange object with an array of the times of the video that have been downloaded. If you just want the percent of the video that's been downloaded, use bufferedPercent. _**see**_: [Buffered Spec](http://dev.w3.org/html5/spec/video.html#dom-media-buffered)

**Returns:** `TimeRange` A mock TimeRange object \(following HTML spec\)

### bufferedEnd <a id="bufferedend"></a>

▸ **bufferedEnd**\(\): `number`

Get the ending time of the last buffered time range This is used in the progress bar to encapsulate all time ranges.

**Returns:** `number` The end of the last buffered time range

### bufferedPercent <a id="bufferedpercent"></a>

▸ **bufferedPercent**\(\): `number`

Get the percent \(as a decimal\) of the video that's been downloaded. This method is not a part of the native HTML video API.

**Returns:** `number` A decimal between 0 and 1 representing the percent that is buffered 0 being 0% and 1 being 100%

### buildCSSClass <a id="buildcssclass"></a>

▸ **buildCSSClass**\(\): `string`

Builds the default DOM class name. Should be overriden by sub-components.

**Returns:** `string` The DOM class name for this object.

### canPlayType <a id="canplaytype"></a>

▸ **canPlayType**\(type: `string`\): "probably" \| "maybe" \| `&quot;&quot;`

Check whether the player can play a given mimetype _**see**_: [https://www.w3.org/TR/2011/WD-html5-20110113/video.html\#dom-navigator-canplaytype](https://www.w3.org/TR/2011/WD-html5-20110113/video.html#dom-navigator-canplaytype)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| type | `string` | `The mimetype to check` |

**Returns:** "probably" \| "maybe" \| `&quot;&quot;`

'probably', 'maybe', or '' \(empty string\)

### cancelAnimationFrame <a id="cancelanimationframe"></a>

▸ **cancelAnimationFrame**\(id: `number`\): `number`

Cancels a queued callback passed to {@link Component\#requestAnimationFrame} \(rAF\).

If you queue an rAF callback via {@link Component\#requestAnimationFrame}, use this function instead of `window.cancelAnimationFrame`. If you don't, your dispose listener will not get cleaned up until {@link Component\#dispose}! _**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/window/cancelAnimationFrame)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| id | `number` | `The rAF ID to clear. The return value of {@link Component#requestAnimationFrame}.` |

**Returns:** `number` Returns the rAF ID that was cleared.

### cancelFullScreen <a id="cancelfullscreen"></a>

▸ **cancelFullScreen**\(\): `Player`

**Returns:** `Player`

### children <a id="children"></a>

▸ **children**\(\): `Component`\[\]

Get an array of all child components

**Returns:** `Component`\[\] The children

### clearInterval <a id="clearinterval"></a>

▸ **clearInterval**\(intervalId: `number`\): `number`

Clears an interval that gets created via `window.setInterval` or {@link Component\#setInterval}. If you set an inteval via {@link Component\#setInterval} use this function instead of `window.clearInterval`. If you don't your dispose listener will not get cleaned up until {@link Component\#dispose}! _**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/clearInterval)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| intervalId | `number` | `The id of the interval to clear. The return value of{@link Component#setInterval} or &#x60;window.setInterval&#x60;.` |

**Returns:** `number` Returns the interval id that was cleared.

### clearTimeout <a id="cleartimeout"></a>

▸ **clearTimeout**\(timeoutId: `number`\): `number`

Clears a timeout that gets created via `window.setTimeout` or {@link Component\#setTimeout}. If you set a timeout via {@link Component\#setTimeout} use this function instead of `window.clearTimout`. If you don't your dispose listener will not get cleaned up until {@link Component\#dispose}! _**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/clearTimeout)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| timeoutId | `number` | `The id of the timeout to clear. The return value of{@link Component#setTimeout} or &#x60;window.setTimeout&#x60;.` |

**Returns:** `number` Returns the timeout id that was cleared.

### contentEl <a id="contentel"></a>

▸ **contentEl**\(\): `Element`

Return the `Component`s DOM element. This is where children get inserted. This will usually be the the same as the element returned in {@link Component\#el}.

**Returns:** `Element` The content element for this `Component`.

### controlText <a id="controltext"></a>

▸ **controlText**\(key: `string`\): `string`

**Parameters:**

| Name | Type |
| :--- | :--- |
| key | `string` |

**Returns:** `string`

### controls <a id="controls"></a>

▸ **controls**\(bool?: `boolean`\): `void`

▸ **controls**\(\): `boolean`

Get or set whether or not the controls are showing. _**fires**_: Player\#controlsenabled

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` bool | `boolean` |

**Returns:** `void` The current value of controls when getting

**Returns:** `boolean`

### createEl <a id="createel"></a>

▸ **createEl**\(\): `Element`

Create the `Player`'s DOM element.

**Returns:** `Element` The DOM element that gets created.

### createModal <a id="createmodal"></a>

▸ **createModal**\(content:  __`string` _\|_ `function` _\|_ `Element` _\|_ `any`_\[\]_, options: `any`\): `ModalDialog`

Creates a simple modal dialog \(an instance of the {@link ModalDialog} component\) that immediately overlays the player with arbitrary content and removes itself when closed. _**check**_:

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| content | `string` \| `function` \| `Element` \| `any`\[\] | `Same as {@link ModalDialog#content}&#x27;s param of the same name.The most straight-forward usage is to provide a string or DOMelement.` |
| options | `any` |  |

**Returns:** `ModalDialog` the {@link ModalDialog} that was created

### currentDimension <a id="currentdimension"></a>

▸ **currentDimension**\(widthOrHeight:  _"width" \| "height"_\): `number`

Get the width or the height of the `Component` elements computed style. Uses `window.getComputedStyle`.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| widthOrHeight | "width" \| "height" | `A string containing &#x27;width&#x27; or &#x27;height&#x27;. Whichever one you want to get.` |

**Returns:** `number` The dimension that gets asked for or 0 if nothing was set for that dimension.

### currentDimensions <a id="currentdimensions"></a>

▸ **currentDimensions**\(\): `DimensionObject`

Get an object that contains width and height values of the `Component`s computed style.

**Returns:** `DimensionObject` The dimensions of the components element

### currentHeight <a id="currentheight"></a>

▸ **currentHeight**\(\): `number`

Get the height of the `Component`s computed style. Uses `window.getComputedStyle`.

**Returns:** `number` height The height of the `Component`s computed style.

### currentSource <a id="currentsource"></a>

▸ **currentSource**\(\): `SourceObject`

Returns the current source object.

**Returns:** `SourceObject` The current source object

### currentSources <a id="currentsources"></a>

▸ **currentSources**\(\): `SourceObject`\[\]

Returns all of the current source objects.

**Returns:** `SourceObject`\[\] The current source objects

### currentSrc <a id="currentsrc"></a>

▸ **currentSrc**\(\): `string`

Returns the fully qualified URL of the current source value e.g. [http://mysite.com/video.mp4](http://mysite.com/video.mp4) Can be used in conjunction with `currentType` to assist in rebuilding the current source object.

**Returns:** `string` The current source

### currentTime <a id="currenttime"></a>

▸ **currentTime**\(seconds: `number`\): `void`

▸ **currentTime**\(\): `number`

Get or set the current time \(in seconds\)

**Parameters:**

| Name | Type |
| :--- | :--- |
| seconds | `number` |

**Returns:** `void`

* the current time in seconds when getting

**Returns:** `number`

### currentType <a id="currenttype"></a>

▸ **currentType**\(\): `string`

Get the current source type e.g. video/mp4 This can allow you rebuild the current source object so that you could load the same source and tech later

**Returns:** `string` The source MIME type

### currentWidth <a id="currentwidth"></a>

▸ **currentWidth**\(\): `number`

Get the width of the `Component`s computed style. Uses `window.getComputedStyle`.

**Returns:** `number` width The width of the `Component`s computed style.

### defaultMuted <a id="defaultmuted"></a>

▸ **defaultMuted**\(defaultMuted: `boolean`\): `void`

▸ **defaultMuted**\(\): `boolean`

Get the current defaultMuted state, or turn defaultMuted on or off. defaultMuted indicates the state of muted on initial playback.

```javascript
  var myPlayer = videojs('some-player-id');

  myPlayer.src("http://www.example.com/path/to/video.mp4");

  // get, should be false
  console.log(myPlayer.defaultMuted());
  // set to true
  myPlayer.defaultMuted(true);
  // get should be true
  console.log(myPlayer.defaultMuted());
```

**Parameters:**

| Name | Type |
| :--- | :--- |
| defaultMuted | `boolean` |

**Returns:** `void`

* true if defaultMuted is on and getting
  * false if defaultMuted is off and getting
  * A reference to the current player when setting

**Returns:** `boolean`

### defaultPlaybackRate <a id="defaultplaybackrate"></a>

▸ **defaultPlaybackRate**\(rate: `number`\): `Player`

▸ **defaultPlaybackRate**\(\): `boolean`

Gets or sets the current default playback rate. A default playback rate of 1.0 represents normal speed and 0.5 would indicate half-speed playback, for instance. defaultPlaybackRate will only represent what the initial playbackRate of a video was, not not the current playbackRate. _**see**_: [https://html.spec.whatwg.org/multipage/embedded-content.html\#dom-media-defaultplaybackrate](https://html.spec.whatwg.org/multipage/embedded-content.html#dom-media-defaultplaybackrate)

**Parameters:**

| Name | Type |
| :--- | :--- |
| rate | `number` |

**Returns:** `Player`

* The default playback rate when getting or 1.0
  * the player when setting

**Returns:** `boolean`

### dimension <a id="dimension"></a>

▸ **dimension**\(dimension:  _"width" \| "height"_, value: `number`\): `void`

▸ **dimension**\(dimension:  _"width" \| "height"_\): `number`

A getter/setter for the `Player`'s width & height.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| dimension | "width" \| "height" | `This string can be:- &#x27;width&#x27;- &#x27;height&#x27;` |
| value | `number` |  |

**Returns:** `void` The dimension arguments value when getting \(width/height\).

**Parameters:**

| Name | Type |
| :--- | :--- |
| dimension | "width" \| "height" |

**Returns:** `number`

### dimensions <a id="dimensions"></a>

▸ **dimensions**\(width:  __`string` _\|_ `number`, height:  __`string` _\|_ `number`\): `void`

Set both the width and height of the `Component` element at the same time.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| width | `string` \| `number` | `Width to set the &#x60;Component&#x60;s element to.` |
| height | `string` \| `number` | `Height to set the &#x60;Component&#x60;s element to.` |

**Returns:** `void`

### dispose <a id="dispose"></a>

▸ **dispose**\(\): `void`

An instance of the `Player` class is created when any of the Video.js setup methods are used to initialize a video.

After an instance has been created it can be accessed globally in two ways:

1. By calling `videojs('example_video_1');`
2. By using it directly via `videojs.players.example_video_1;`

**Returns:** `void`

### duration <a id="duration"></a>

▸ **duration**\(seconds: `number`\): `void`

▸ **duration**\(\): `number`

Normally gets the length in time of the video in seconds; in all but the rarest use cases an argument will NOT be passed to the method

> **NOTE**: The video must have started loading before the duration can be known, and in the case of Flash, may not be known until the video starts playing. _**fires**_: Player\#durationchange

**Parameters:**

| Name | Type |
| :--- | :--- |
| seconds | `number` |

**Returns:** `void`

* The duration of the video in seconds when getting

**Returns:** `number`

### el <a id="el"></a>

▸ **el**\(\): `Element`

Get the `Component`s DOM element

**Returns:** `Element` The DOM element for this `Component`.

### emitTapEvents <a id="emittapevents"></a>

▸ **emitTapEvents**\(\): `void`

Emit a 'tap' events when touch event support gets detected. This gets used to support toggling the controls through a tap on the video. They get enabled because every sub-component would have extra overhead otherwise. _**fires**_: Component\#tap

_**listens**_: Component\#touchstart

_**listens**_: Component\#touchmove

_**listens**_: Component\#touchleave

_**listens**_: Component\#touchcancel

_**listens**_: Component\#touchend

**Returns:** `void`

### enableTouchActivity <a id="enabletouchactivity"></a>

▸ **enableTouchActivity**\(\): `void`

This function reports user activity whenever touch events happen. This can get turned off by any sub-components that wants touch events to act another way.

Report user touch activity when touch events occur. User activity gets used to determine when controls should show/hide. It is simple when it comes to mouse events, because any mouse event should show the controls. So we capture mouse events that bubble up to the player and report activity when that happens. With touch events it isn't as easy as `touchstart` and `touchend` toggle player controls. So touch events can't help us at the player level either.

User activity gets checked asynchronously. So what could happen is a tap event on the video turns the controls off. Then the `touchend` event bubbles up to the player. Which, if it reported user activity, would turn the controls right back on. We also don't want to completely block touch events from bubbling up. Furthermore a `touchmove` event and anything other than a tap, should not turn controls back on. _**listens**_: Component\#touchstart

_**listens**_: Component\#touchmove

_**listens**_: Component\#touchend

_**listens**_: Component\#touchcancel

**Returns:** `void`

### ended <a id="ended"></a>

▸ **ended**\(\): `boolean`

Get the value of `ended` from the media element. `ended` indicates whether the media has reached the end or not. _**see**_: [Spec](https://www.w3.org/TR/html5/embedded-content-0.html#dom-media-ended)

**Returns:** `boolean`

* The value of `ended` from the media element.
  * True indicates that the media has ended.
  * False indicates that the media has not ended.

### enterFullWindow <a id="enterfullwindow"></a>

▸ **enterFullWindow**\(\): `void`

When fullscreen isn't supported we can stretch the video container to as wide as the browser will let us. _**fires**_: Player\#enterFullWindow

**Returns:** `void`

### error <a id="error"></a>

▸ **error**\(err:  __`MediaError` _\|_ `string` _\|_ `number` _\|_ `null`\): `void`

▸ **error**\(\): `MediaError` \| `null`

Set or get the current MediaError _**fires**_: Player\#error

**Parameters:**

| Name | Type |
| :--- | :--- |
| err | `MediaError` \| `string` \| `number` \| `null` |

**Returns:** `void` The current MediaError when getting \(or null\)

**Returns:** `MediaError` \| `null`

### exitFullWindow <a id="exitfullwindow"></a>

▸ **exitFullWindow**\(\): `void`

Exit full window _**fires**_: Player\#exitFullWindow

**Returns:** `void`

### exitFullscreen <a id="exitfullscreen"></a>

▸ **exitFullscreen**\(\): `Player`

Return the video to its normal size after having been in full screen mode _**fires**_: Player\#fullscreenchange //noinspection JSUnresolvedVariable

**Returns:** `Player`

### fluid <a id="fluid"></a>

▸ **fluid**\(bool: `boolean`\): `void`

▸ **fluid**\(\): `boolean`

A getter/setter/toggler for the vjs-fluid `className` on the `Player`.

**Parameters:**

| Name | Type |
| :--- | :--- |
| bool | `boolean` |

**Returns:** `void`

* The value of fluid when getting.
  * `undefined` when setting.

**Returns:** `boolean`

### focus <a id="focus"></a>

▸ **focus**\(\): `void`

Set the focus to this component

**Returns:** `void`

### getAttribute <a id="getattribute"></a>

▸ **getAttribute**\(attribute: `string`\): `string` \| `null`

Get the value of an attribute on the `Component`s element. _**see**_: [DOM API](https://developer.mozilla.org/en-US/docs/Web/API/Element/getAttribute)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| attribute | `string` | `Name of the attribute to get the value from.` |

**Returns:** `string` \| `null`

* The value of the attribute that was asked for.
  * Can be an empty string on some browsers if the attribute does not exist

    or has no value

  * Most browsers will return null if the attibute does not exist or has

    no value.

### getCache <a id="getcache"></a>

▸ **getCache**\(\): `any`

Get object for cached values.

**Returns:** `any` get the current object cache

### getChild <a id="getchild"></a>

▸ **getChild**\(name: `string`\): `Component` \| `undefined`

Returns the child `Component` with the given `name`.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| name | `string` | `The name of the child &#x60;Component&#x60; to get.` |

**Returns:** `Component` \| `undefined`

The child `Component` with the given `name` or undefined.

### getChildById <a id="getchildbyid"></a>

▸ **getChildById**\(id: `string`\): `Component` \| `undefined`

Returns the child `Component` with the given `id`.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| id | `string` | `The id of the child &#x60;Component&#x60; to get.` |

**Returns:** `Component` \| `undefined`

The child `Component` with the given `id` or undefined.

### getVideoPlaybackQuality <a id="getvideoplaybackquality"></a>

▸ **getVideoPlaybackQuality**\(\): `any`

Gets available media playback quality metrics as specified by the W3C's Media Playback Quality API. _**see**_: [Spec](https://wicg.github.io/media-playback-quality)

**Returns:** `any` An object with supported media playback quality metrics or undefined if there is no tech or the tech does not support it.

### hasClass <a id="hasclass"></a>

▸ **hasClass**\(classToCheck: `string`\): `boolean`

Check if a component's element has a CSS class name.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| classToCheck | `string` | `CSS class name to check.` |

**Returns:** `boolean`

* True if the `Component` has the class.
  * False if the `Component` does not have the class\`

### hasPlugin <a id="hasplugin"></a>

▸ **hasPlugin**\(name: `string`\): `boolean`

Reports whether or not a player has a plugin available.

This does not report whether or not the plugin has ever been initialized on this player. For that, \[usingPlugin\]{@link Player\#usingPlugin}.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| name | `string` | `The name of a plugin.` |

**Returns:** `boolean` Whether or not this player has the requested plugin available.

### hasStarted <a id="hasstarted"></a>

▸ **hasStarted**\(request: `boolean`\): `void`

▸ **hasStarted**\(\): `boolean`

Add/remove the vjs-has-started class _**fires**_: Player\#firstplay

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| request | `boolean` | `- true: adds the class- false: remove the class` |

**Returns:** `void` the boolean value of hasStarted\_

**Returns:** `boolean`

### height <a id="height"></a>

▸ **height**\(value: `number`\): `void`

▸ **height**\(\): `number`

A getter/setter for the `Player`'s height. Returns the player's configured value. To get the current height use `currentheight()`.

**Parameters:**

| Name | Type |
| :--- | :--- |
| value | `number` |

**Returns:** `void` The current height of the `Player` when getting.

**Returns:** `number`

### hide <a id="hide"></a>

▸ **hide**\(\): `void`

Hide the `Component`s element if it is currently showing by adding the 'vjs-hidden\` class name to it.

**Returns:** `void`

### id <a id="id"></a>

▸ **id**\(\): `string`

Get this `Component`s ID

**Returns:** `string` The id of this `Component`

### initChildren <a id="initchildren"></a>

▸ **initChildren**\(\): `void`

Add and initialize default child `Component`s based upon options.

**Returns:** `void`

### isAudio <a id="isaudio"></a>

▸ **isAudio**\(bool: `boolean`\): `void`

▸ **isAudio**\(\): `boolean`

Gets or sets the audio flag

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| bool | `boolean` | `- true signals that this is an audio player- false signals that this is not an audio player` |

**Returns:** `void` The current value of isAudio when getting

**Returns:** `boolean`

### isFullscreen <a id="isfullscreen"></a>

▸ **isFullscreen**\(isFS: `boolean`\): `void`

▸ **isFullscreen**\(\): `boolean`

Check if the player is in fullscreen mode or tell the player that it is or is not in fullscreen mode.

> NOTE: As of the latest HTML5 spec, isFullscreen is no longer an official property and instead document.fullscreenElement is used. But isFullscreen is still a valuable property for internal player workings.

**Parameters:**

| Name | Type |
| :--- | :--- |
| isFS | `boolean` |

**Returns:** `void`

* true if fullscreen is on and getting
  * false if fullscreen is off and getting

**Returns:** `boolean`

### language <a id="language"></a>

▸ **language**\(code: `string`\): `void`

▸ **language**\(\): `string`

The player's language code NOTE: The language should be set in the player options if you want the the controls to be built with a specific language. Changing the language later will not update controls text.

**Parameters:**

| Name | Type |
| :--- | :--- |
| code | `string` |

**Returns:** `void` The current language code when getting

**Returns:** `string`

### languageSwitch <a id="languageswitch"></a>

▸ **languageSwitch**\(options: `any`\): `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| options | `any` |

**Returns:** `void`

### languages <a id="languages"></a>

▸ **languages**\(\): `string`\[\]

Get the player's language dictionary Merge every time, because a newly added plugin might call videojs.addLanguage\(\) at any time Languages specified directly in the player options have precedence

**Returns:** `string`\[\] An array of of supported languages

### load <a id="load"></a>

▸ **load**\(\): `void`

Begin loading the src data.

**Returns:** `void`

### localize <a id="localize"></a>

▸ **localize**\(string: `string`, tokens?: `string`_\[\]_, defaultValue?: `string`\): `string`

Localize a string given the string in english.

If tokens are provided, it'll try and run a simple token replacement on the provided string. The tokens it looks for look like `{1}` with the index being 1-indexed into the tokens array.

If a `defaultValue` is provided, it'll use that over `string`, if a value isn't found in provided language files. This is useful if you want to have a descriptive key for token replacement but have a succinct localized string and not require `en.json` to be included.

Currently, it is used for the progress bar timing.

```javascript
{
  "progress bar timing: currentTime={1} duration={2}": "{1} of {2}"
}
```

It is then used like so:

```javascript
this.localize('progress bar timing: currentTime={1} duration{2}',
              [this.player_.currentTime(), this.player_.duration()],
              '{1} of {2}');
```

Which outputs something like: `01:23 of 24:56`.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| string | `string` | `The string to localize and the key to lookup in the language files.` |
| `Optional` tokens | `string`\[\] |  |
| `Optional` defaultValue | `string` |  |

**Returns:** `string` The localized string or if no localization exists the english string.

### lockShowing <a id="lockshowing"></a>

▸ **lockShowing**\(\): `void`

Lock a `Component`s element in its visible state by adding the 'vjs-lock-showing' class name to it. Used during fadeIn/fadeOut.

**Returns:** `void`

### loop <a id="loop"></a>

▸ **loop**\(value?: `boolean`\): `void`

▸ **loop**\(\): `string`

Get or set the loop attribute on the video element.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` value | `boolean` |

**Returns:** `void` The current value of loop when getting

**Returns:** `string`

### muted <a id="muted"></a>

▸ **muted**\(muted: `boolean`\): `void`

▸ **muted**\(\): `boolean`

Get the current muted state, or turn mute on or off

**Parameters:**

| Name | Type |
| :--- | :--- |
| muted | `boolean` |

**Returns:** `void`

* true if mute is on and getting
  * false if mute is off and getting

**Returns:** `boolean`

### name <a id="name"></a>

▸ **name**\(\): `string`

Get the `Component`s name. The name gets used to reference the `Component` and is set during registration.

**Returns:** `string` The name of this `Component`.

### off <a id="off"></a>

▸ **off**\(target?:  __`Component` _\|_ `Element`, type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

▸ **off**\(type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

Removes listener\(s\) from event\(s\) on an evented object.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` target | `Component` \| `Element` |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

### on <a id="on"></a>

▸ **on**\(target?:  __`Component` _\|_ `Element`, type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

▸ **on**\(type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

Add a listener to an event \(or events\) on this object or another evented object.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` target | `Component` \| `Element` |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

### one <a id="one"></a>

▸ **one**\(target?:  __`Component` _\|_ `Element`, type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

▸ **one**\(type?:  __`string` _\|_ `string`_\[\]_, listener?: `function`\): `void`

Add a listener to an event \(or events\) on this object or another evented object. The listener will only be called once and then removed.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` target | `Component` \| `Element` |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` type | `string` \| `string`\[\] |
| `Optional` listener | `function` |

**Returns:** `void`

### options <a id="options"></a>

▸ **options**\(obj: `any`\): `any`

Deep merge of options objects with new options.

> Note: When both `obj` and `options` contain properties whose values are objects. The two properties get merged using {@link module:mergeOptions} _**deprecated**_: since version 5

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| obj | `any` | `The object that contains new options.` |

**Returns:** `any` A new object of `this.options_` and `obj` merged together.

### pause <a id="pause"></a>

▸ **pause**\(\): `Player`

Pause the video playback _**check**_:

**Returns:** `Player` A reference to the player object this function was called on

### paused <a id="paused"></a>

▸ **paused**\(\): `boolean`

Check if the player is paused or has yet to play

**Returns:** `boolean`

* false: if the media is currently playing
  * true: if media is not currently playing

### play <a id="play"></a>

▸ **play**\(\): `Promise`&lt;`void`&gt; \| `undefined`

Attempt to begin playback at the first opportunity. _**check**_:

**Returns:** `Promise`&lt;`void`&gt; \| `undefined`

Returns a `Promise` only if the browser returns one and the player is ready to begin playback. For some browsers and all non-ready situations, this will return `undefined`.

### playbackRate <a id="playbackrate"></a>

▸ **playbackRate**\(rate?: `number`\): `void`

▸ **playbackRate**\(\): `number`

Gets or sets the current playback rate. A playback rate of 1.0 represents normal speed and 0.5 would indicate half-speed playback, for instance. _**see**_: [https://html.spec.whatwg.org/multipage/embedded-content.html\#dom-media-playbackrate](https://html.spec.whatwg.org/multipage/embedded-content.html#dom-media-playbackrate)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` rate | `number` |

**Returns:** `void` The current playback rate when getting or 1.0

**Returns:** `number`

### played <a id="played"></a>

▸ **played**\(\): `any`

Get a TimeRange object representing the current ranges of time that the user has played. _**check**_:

**Returns:** `any` A time range object that represents all the increments of time that have been played.

### player <a id="player-1"></a>

▸ **player**\(\): `Player`

Return the [Player](annotoplayer.playerimplementation.md#player) that the `Component` has attached to.

**Returns:** `Player` The player that this `Component` has attached to.

### playsinline <a id="playsinline"></a>

▸ **playsinline**\(value: `boolean`\): `Player`

▸ **playsinline**\(\): `string`

Set or unset the playsinline attribute. Playsinline tells the browser that non-fullscreen playback is preferred. _**see**_: [Spec](https://html.spec.whatwg.org/#attr-video-playsinline)

**Parameters:**

| Name | Type |
| :--- | :--- |
| value | `boolean` |

**Returns:** `Player`

* the current value of playsinline
  * the player when setting

**Returns:** `string`

### poster <a id="poster"></a>

▸ **poster**\(src: `string`\): `void`

▸ **poster**\(\): `string`

Get or set the poster image source url _**fires**_: Player\#posterchange

**Parameters:**

| Name | Type |
| :--- | :--- |
| src | `string` |

**Returns:** `void` The current value of poster when getting

**Returns:** `string`

### preload <a id="preload"></a>

▸ **preload**\(value?: `boolean`\): `string`

Get or set the preload attribute

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` value | `boolean` |

**Returns:** `string` The preload attribute value when getting

### ready <a id="ready"></a>

▸ **ready**\(callback: `function`\): `this`

Bind a listener to the component's ready state. Different from event listeners in that if the ready event has already happened it will trigger the function immediately.

**Parameters:**

| Name | Type |
| :--- | :--- |
| callback | `function` |

**Returns:** `this` Returns itself; method can be chained.

### remainingTime <a id="remainingtime"></a>

▸ **remainingTime**\(\): `number`

Calculates how much time is left in the video. Not part of the native video API.

**Returns:** `number` The time remaining in seconds

### remainingTimeDisplay <a id="remainingtimedisplay"></a>

▸ **remainingTimeDisplay**\(\): `number`

A remaining time function that is intented to be used when the time is to be displayed directly to the user.

**Returns:** `number` The rounded time remaining in seconds

### remoteTextTracks <a id="remotetexttracks"></a>

▸ **remoteTextTracks**\(\): `TextTrackList`

Get the remote {@link TextTrackList}

**Returns:** `TextTrackList` The current remote text track list

### removeAttribute <a id="removeattribute"></a>

▸ **removeAttribute**\(attribute: `string`\): `void`

Remove an attribute from the `Component`s element. _**see**_: [DOM API](https://developer.mozilla.org/en-US/docs/Web/API/Element/removeAttribute)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| attribute | `string` | `Name of the attribute to remove.` |

**Returns:** `void`

### removeChild <a id="removechild"></a>

▸ **removeChild**\(component: `Component`\): `void`

Remove a child `Component` from this `Component`s list of children. Also removes the child `Component`s element from this `Component`s element.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| component | `Component` | `The child &#x60;Component&#x60; to remove.` |

**Returns:** `void`

### removeClass <a id="removeclass"></a>

▸ **removeClass**\(classToRemove: `string`\): `void`

Remove a CSS class name from the `Component`s element.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| classToRemove | `string` | `CSS class name to remove` |

**Returns:** `void`

### removeRemoteTextTrack <a id="removeremotetexttrack"></a>

▸ **removeRemoteTextTrack**\(track: `HTMLTrackElement`\): `void`

Remove a remote {@link TextTrack} from the respective {@link TextTrackList} and {@link HtmlTrackElementList}.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| track | `HTMLTrackElement` | `Remote {@link TextTrack} to remove` |

**Returns:** `void` does not return anything

### reportUserActivity <a id="reportuseractivity"></a>

▸ **reportUserActivity**\(event: `any`\): `void`

Report user activity

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| event | `any` | `Event object` |

**Returns:** `void`

### requestAnimationFrame <a id="requestanimationframe"></a>

▸ **requestAnimationFrame**\(fn: `Component.GenericCallback`\): `number`

Queues up a callback to be passed to requestAnimationFrame \(rAF\), but with a few extra bonuses:

* Supports browsers that do not support rAF by falling back to {@link Component\#setTimeout}.
* The callback is turned into a {@link Component~GenericCallback} \(i.e. bound to the component\).
* Automatic cancellation of the rAF callback is handled if the component is disposed before it is called. _**listens**_: Component\#dispose

_**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| fn | `Component.GenericCallback` | `A function that will be bound to this component and executed justbefore the browser&#x27;s next repaint.` |

**Returns:** `number` Returns an rAF ID that gets used to identify the timeout. It can also be used in {@link Component\#cancelAnimationFrame} to cancel the animation frame callback.

### requestFullscreen <a id="requestfullscreen"></a>

▸ **requestFullscreen**\(\): `Player`

Increase the size of the video to full screen In some browsers, full screen is not supported natively, so it enters "full window mode", where the video fills the browser window. In browsers and devices that support native full screen, sometimes the browser's default controls will be shown, and not the Video.js custom skin. This includes most mobile devices \(iOS, Android\) and older versions of Safari. _**fires**_: Player\#fullscreenchange

**Returns:** `Player`

### reset <a id="reset"></a>

▸ **reset**\(\): `void`

Reset the player. Loads the first tech in the techOrder, and calls `reset` on the tech\`.

**Returns:** `void`

### scrubbing <a id="scrubbing"></a>

▸ **scrubbing**\(isScrubbing: `boolean`\): `void`

▸ **scrubbing**\(\): `boolean`

Returns whether or not the user is "scrubbing". Scrubbing is when the user has clicked the progress bar handle and is dragging it along the progress bar.

**Parameters:**

| Name | Type |
| :--- | :--- |
| isScrubbing | `boolean` |

**Returns:** `void` The value of scrubbing when getting

**Returns:** `boolean`

### seekable <a id="seekable"></a>

▸ **seekable**\(\): `TimeRanges`

Returns the TimeRanges of the media that are currently available for seeking to.

**Returns:** `TimeRanges` TimeRanges Returns the TimeRanges of the media that are currently available for seeking to.

### seeking <a id="seeking"></a>

▸ **seeking**\(\): `boolean`

Returns whether or not the player is in the "seeking" state.

**Returns:** `boolean` boolean True if the player is in the seeking state, false if not.

### selectSource <a id="selectsource"></a>

▸ **selectSource**\(sources: `any`_\[\]_\): `any`

Select source based on tech-order or source-order Uses source-order selection if `options.sourceOrder` is truthy. Otherwise, defaults to tech-order selection

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| sources | `any`\[\] | `The sources for a media asset` |

**Returns:** `any` Object of source and tech order or false

### setAttribute <a id="setattribute"></a>

▸ **setAttribute**\(attribute: `string`, value: `string`\): `void`

Set the value of an attribute on the `Component`'s element _**see**_: [DOM API](https://developer.mozilla.org/en-US/docs/Web/API/Element/setAttribute)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| attribute | `string` | `Name of the attribute to set.` |
| value | `string` | `Value to set the attribute to.` |

**Returns:** `void`

### setInterval <a id="setinterval"></a>

▸ **setInterval**\(fn: `Component.GenericCallback`, interval: `number`\): `number`

Creates a function that gets run every `x` milliseconds. This function is a wrapper around `window.setInterval`. There are a few reasons to use this one instead though.

1. It gets cleared via {@link Component\#clearInterval} when {@link Component\#dispose} gets called.
2. The function callback will be a {@link Component~GenericCallback}

   _**listens**_: Component\#dispose

_**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/setInterval)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| fn | `Component.GenericCallback` | `The function to run every &#x60;x&#x60; seconds.` |
| interval | `number` | `Execute the specified function every &#x60;x&#x60; milliseconds.` |

**Returns:** `number` Returns an id that can be used to identify the interval. It can also be be used in {@link Component\#clearInterval} to clear the interval.

### setTimeout <a id="settimeout"></a>

▸ **setTimeout**\(fn: `Component.GenericCallback`, timeout: `number`\): `number`

Creates a function that runs after an `x` millisecond timeout. This function is a wrapper around `window.setTimeout`. There are a few reasons to use this one instead though:

1. It gets cleared via {@link Component\#clearTimeout} when {@link Component\#dispose} gets called.
2. The function callback will gets turned into a {@link Component~GenericCallback}

> Note: You can't use `window.clearTimeout` on the id returned by this function. This will cause its dispose listener not to get cleaned up! Please use {@link Component\#clearTimeout} or {@link Component\#dispose} instead. _**listens**_: Component\#dispose

_**see**_: [Similar to](https://developer.mozilla.org/en-US/docs/Web/API/WindowTimers/setTimeout)

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| fn | `Component.GenericCallback` | `The function that will be run after &#x60;timeout&#x60;.` |
| timeout | `number` | `Timeout in milliseconds to delay before executing the specified function.` |

**Returns:** `number` Returns a timeout ID that gets used to identify the timeout. It can also get used in {@link Component\#clearTimeout} to clear the timeout that was set.

### show <a id="show"></a>

▸ **show**\(\): `void`

Show the `Component`s element if it is hidden by removing the 'vjs-hidden' class name from it.

**Returns:** `void`

### src <a id="src"></a>

▸ **src**\(source:  __`string` _\|_ `SourceObject` _\|_ `SourceObject`_\[\]_\): `void`

▸ **src**\(\): `string`

Get or set the video source.

**Parameters:**

| Name | Type |
| :--- | :--- |
| source | `string` \| `SourceObject` \| `SourceObject`\[\] |

**Returns:** `void` If the `source` argument is missing, returns the current source URL. Otherwise, returns nothing/undefined.

**Returns:** `string`

### supportsFullScreen <a id="supportsfullscreen"></a>

▸ **supportsFullScreen**\(\): `boolean`

Check if current tech can support native fullscreen \(e.g. with built in controls like iOS, so not our flash swf\)

**Returns:** `boolean` if native fullscreen is supported

### tech <a id="tech"></a>

▸ **tech**\(safety?: `any`\): `Tech`

Return a reference to the current {@link Tech}. It will print a warning by default about the danger of using the tech directly but any argument that is passed in will silence the warning.

**Parameters:**

| Name | Type |
| :--- | :--- |
| `Optional` safety | `any` |

**Returns:** `Tech` The Tech

### textTracks <a id="texttracks"></a>

▸ **textTracks**\(\): `TextTrackList`

Get the remote {@link TextTrackList}

**Returns:** `TextTrackList` The current remote text track list

### toJSON <a id="tojson"></a>

▸ **toJSON**\(\): `any`

returns a JavaScript object reperesenting the current track information. **DOES not return it as JSON**

**Returns:** `any` Object representing the current of track info

### toggleClass <a id="toggleclass"></a>

▸ **toggleClass**\(classToToggle: `string`, predicate?:  __`boolean` _\|_ `Dom.Predicate`\): `void`

Add or remove a CSS class name from the component's element.

* `classToToggle` gets added when {@link Component\#hasClass} would return false.
* `classToToggle` gets removed when {@link Component\#hasClass} would return true.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| classToToggle | `string` | `The class to add or remove based on (@link Component#hasClass}` |
| `Optional` predicate | `boolean` \| `Dom.Predicate` |  |

**Returns:** `void`

### trigger <a id="trigger"></a>

▸ **trigger**\(event: `any`, hash?: `any`\): `boolean`

Fire an event on this evented object, causing its listeners to be called.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| event | `any` | `An event type or an object with a type property.` |
| `Optional` hash | `any` |  |

**Returns:** `boolean` Whether or not the default behavior was prevented.

### triggerReady <a id="triggerready"></a>

▸ **triggerReady**\(\): `void`

Trigger all the ready listeners for this `Component`. _**fires**_: Component\#ready

**Returns:** `void`

### unlockShowing <a id="unlockshowing"></a>

▸ **unlockShowing**\(\): `void`

Unlock a `Component`s element from its visible state by removing the 'vjs-lock-showing' class name from it. Used during fadeIn/fadeOut.

**Returns:** `void`

### userActive <a id="useractive"></a>

▸ **userActive**\(bool: `boolean`\): `void`

▸ **userActive**\(\): `boolean`

Get/set if user is active _**fires**_: Player\#useractive

_**fires**_: Player\#userinactive

**Parameters:**

| Name | Type |
| :--- | :--- |
| bool | `boolean` |

**Returns:** `void` The current value of userActive when getting

**Returns:** `boolean`

### usingNativeControls <a id="usingnativecontrols"></a>

▸ **usingNativeControls**\(bool: `boolean`\): `void`

▸ **usingNativeControls**\(\): `boolean`

Toggle native controls on/off. Native controls are the controls built into devices \(e.g. default iPhone controls\), Flash, or other techs \(e.g. Vimeo Controls\) **This should only be set by the current tech, because only the tech knows if it can support native controls** _**fires**_: Player\#usingnativecontrols

_**fires**_: Player\#usingcustomcontrols

**Parameters:**

| Name | Type |
| :--- | :--- |
| bool | `boolean` |

**Returns:** `void` The current value of native controls when getting

**Returns:** `boolean`

### usingPlugin <a id="usingplugin"></a>

▸ **usingPlugin**\(name: `string`\): `boolean`

Reports whether or not a player is using a plugin by name.

For basic plugins, this only reports whether the plugin has _ever_ been initialized on this player.

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| name | `string` | `The name of a plugin.` |

**Returns:** `boolean` Whether or not this player is using the requested plugin.

### videoHeight <a id="videoheight"></a>

▸ **videoHeight**\(\): `number`

Get video height

**Returns:** `number` current video height

### videoWidth <a id="videowidth"></a>

▸ **videoWidth**\(\): `number`

Get video width

**Returns:** `number` current video width

### volume <a id="volume"></a>

▸ **volume**\(percentAsDecimal: `number`\): `TimeRange`

▸ **volume**\(\): `number`

Get or set the current volume of the media

**Parameters:**

| Name | Type |
| :--- | :--- |
| percentAsDecimal | `number` |

**Returns:** `TimeRange` The current volume as a percent when getting

**Returns:** `number`

### width <a id="width"></a>

▸ **width**\(value: `number`\): `void`

▸ **width**\(\): `number`

A getter/setter for the `Player`'s width. Returns the player's configured value. To get the current width use `currentWidth()`.

**Parameters:**

| Name | Type |
| :--- | :--- |
| value | `number` |

**Returns:** `void` The current width of the `Player` when getting.

**Returns:** `number`

