# An old-school flashlight

There are a surprising amount of flashlight apps on the iOS and Android app stores, many of which are full of malware and/or ads.

However, given that a flashlight is in many cases just the white screen of the device, we can take some inspiration from a [Hacker News](https://news.ycombinator.com) thread I read but have since lost the link for and create a web page with a white background that switches to black (and back) when you tap your screen.

# The code

You can use a ([data URI](https://en.wikipedia.org/wiki/Data_URI_scheme)) in a browser to accomplish the gist of the flashlight functionality.

```data:text/html;charset=utf-8,<!DOCTYPE html><title>Flashlight</title><html onclick="on=!on;this.style.background=on?'white':'black'"><body onload=on=true>```

Furthermore, you could even turn this into a QR code.


![](flashlight-qr-code.gif)

Now, if you scan that QR code and paste the result into a browser you should have a fully functional flashlight from your device screen with no malware or ads.

# Using it as an app

If you want to go one step further and have this capability available on your home screen like any other app, it's not hard to do.  In iOS for example, once you have the page up in Safari you can add it to your home screen.  Now you have a flashlight 'app.'