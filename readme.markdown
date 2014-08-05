# svg-to-canvas

svg to canvas

Try it out! [![view on requirebin](http://requirebin.com/badge.png)](http://requirebin.com/?gist=45f32c2c85ea7894956f)

use with [browserify](http://browserify.org)

# methods

``` js
var convert = require('svg-to-canvas');
var svg = document.querySelector('svg');

convert(svg, function thumbnail(canvas) {
  image.onload = function() {
    image.setAttribute('height', image.height*0.3);
    image.setAttribute('width', image.width*0.3);
    window.document.body.appendChild(image);
  };
  image.src = canvas.toDataURL();
  var image = new Image();
});
```

# install

With [npm](https://npmjs.org) do:

```
npm install svg-to-canvas
```

# license

MIT
