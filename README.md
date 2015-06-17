#X# SS-Handler
Node Package Manager (NPM) Module.
Consisting of a couple utility methods for escaping and unescaping HTML entities – commonly needed utils to prevent XSS attacks when rendering user generated content.

## Installation
  npm install xss-handler --save

## Usage
  var xss-handler = require('xss-handler')
      escape = xss-handler.escape,
      unescape = xss-handler.unescape;
  var html = '< h1>Hello World</h1 >',
      escaped = escape(html),
      unescaped = unescape(escaped);
  console.log('html', html, 'escaped', escaped, 'unescaped', unescaped);

## Read More:
XSS: http://www.acunetix.com/websitesecurity/cross-site-scripting/
Module: https://quickleft.com/blog/creating-and-publishing-a-node-js-module/
