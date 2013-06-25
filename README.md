BgImgLoader
===========

A small plugin for loading CSS background images with callback. This allows you to load the image in programmatically and then respond to it OnLoad event via a callback. The plugin will load the image from the URI of a data attribute on the element (default is "data-bg-src")

Options
---

srcAttr: The data attribute containing the URL of the image to load. (default: "data-bg-src)
callback: Function to call when the image has loaded and been applied to the 'background-image' CSS attribute of the element.

Usage
---

$(".element").bgImgLoad({
  srcAttr: "data-img-url",
  callback: function(){
    $(this).addClass("loaded");
  }
});
