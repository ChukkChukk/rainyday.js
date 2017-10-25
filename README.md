# rainyday.js

[![Build Status](https://travis-ci.org/maroslaw/rainyday.js.svg?branch=master)](https://travis-ci.org/maroslaw/rainyday.js)
[![Dependency Status](https://img.shields.io/david/maroslaw/rainyday.js.svg)](https://david-dm.org/maroslaw/rainyday.js)
[![npm](https://img.shields.io/npm/dm/thepiratebay.svg?maxAge=2592000)]()

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XWP2SR3FLGE6C)

A simple script for simulating raindrops falling on a glass surface.

For demos and more information see the [project page](http://maroslaw.github.io/rainyday.js/).

## How to use

```js
var engine = new RainyDay({
    image: element,         // [Image Id or Image element itself, Id of Element having background Image or Element itself]
                            // This value is required
    parentElement: someDiv, // Element to be used as a parent for the canvas
                            // If not provided assuming the 'body' element
    crop: [0, 0, 50, 60],   // Coordinates if only a part of the image should be used
                            // If not provided entire image will be used
    blur: 10,               // Defines blur due to rain effect
                            // Assuming 10 if not provided
                            // Use 0 value to disable the blur
    opacity: 1              // Opacity of rain drops
                            // Assuming 1 if not provided
});
```
