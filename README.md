# jQuery Pop Window Plugin

A super simple jQuery plugin for popup windows. Tested in IE7+, FF, Safari and Chrome.

## Installation

Download the [`jquery.popupwindow.js`](https://github.com/mkdynamic/jquery-popupwindow/raw/master/jquery.popupwindow.js) file to your project, and add to your page after including jQuery:

```html
<script src="jquery.js" type="text/javascript"></script>
<script src="jquery.popupwindow.js" type="text/javascript"></script>
```

Checkout this [example](https://github.com/mkdynamic/jquery-popupwindow/raw/master/example.html).

## Basic Usage

To open a popup window:

```javascript
$.popupWindow('http://google.com');
```

By default this will open a 500x500 pixel window which is auto-centered and has minimal chrome.

## Options

Here's an example showing the full list of the options you can set:

```javascript
$.popupWindow('http://google.com', {
    height: 300,
    width: 200,
    toolbar: false,
    scrollbars: false, // safari always adds scrollbars
    status: false,
    resizable: true,
    left: 100,
    top: 100,
    center: false, // auto-center
    createNew: true, // open a new window, or re-use existing popup
    location: false,
    menubar: false,
    onUnload: function() { // callback when window closes
        alert('Window closed!');
    } 
});
```
