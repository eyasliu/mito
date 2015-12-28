# mito v1.0.0

> micro-templating function

This is forked from John Resig's [micro-templating](http://ejohn.org/blog/javascript-micro-templating/).

# Syntax

Similar to `.ejs`

```ejs
<html>
  <head>
    <title></title>
  </head>
  <body>
    <ul>
      <% items.forEach(function (item) { %>
        <li><a href="<%= item.url %>"><%= item.name %></a></li>
      <% }) %>
    </ul>
  </body>
</html>
```

# API

```js
var mito = require('mito')
```

## mito(str)

- @param {String} str The template string

Returns template function compiled with the given template string.

## mito(str)(obj)

- @param {Object} obj The template parameter

Returns the rendered string with template parameter

# Feature

- 266B minified
- No cache mechanism
- No include/import/require support

# License

MIT
