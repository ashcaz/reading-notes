# Mustache and Flexbox

Links:

1. [Templating with Mustche](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)
2. [A Guide to Flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
3. [Flexbox Froggy](https://flexboxfroggy.com/)
4. [Mustache.js Official Documentation](https://github.com/janl/mustache.js)

## Mustache Templating


HTML Mustcahe Template:

```HTML
<html>
  <body onload="renderHello()">
    <div id="target">Loading...</div>
    <script id="template" type="x-tmpl-mustache">
      Hello {{ name }}!
    </script>

    <script src="https://unpkg.com/mustache@latest"></script>
    <script src="render.js"></script>
  </body>
</html>
```
JavaScript:

```JavaScript
function renderHello() {
  var template = document.getElementById('template').innerHTML;
  var rendered = Mustache.render(template, { name: 'Luke' });
  document.getElementById('target').innerHTML = rendered;
}
```

[Back to Homepage](https://ashcaz.github.io/reading-notes)