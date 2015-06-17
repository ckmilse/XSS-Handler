## XSS-Handler
Node Package Manager (NPM) Module.
Consisting of a couple utility methods for escaping and unescaping HTML entities – commonly needed utils to prevent XSS attacks when rendering user generated content.

## Installation
If it was published you could use: 
  npm install xss-handler --save
But I'm not publishing, so, you should use:
  npm install https://github.com/angelcambero/NPM-Module-XSS.git --save

Note that --save would add the package as a dependecy to the package.json file of the project where you install this package.



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
