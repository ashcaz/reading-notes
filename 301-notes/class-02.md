## Duckett JS jQuery (p.293-301,306-331,354-357)

**What is jQuery?**

jQuery is a JavaScript file that you include in your web pages. It lets you find elements using CSS-style selectors and then do something with the elements using jQuery methods

`$('li.hot')` 

This selector finads all the `<li>` elements with the class of hot.


*Similarities to DOM*

  - jQuery selectors performa similar task to traditional DOM queries, but the syntax is simpler
  - you can store the jQuery object in a variable, just like with DOM nodes
  - You can use jQuery methods and properties to manipulate the DOM nodes that you slect.

**Why Use jQuery?**

1. Simple selectors
2. Common tasks in less code
3. Cross-browser compatibility

![Single Element vs Multiple elements](../img/jquery-elements)

**Checking A Page Is Ready To Work With**

![.ready()](../img/ready)


The `.ready()` method checks if the browser supports the `DOMCntentLoaded` event, because it fires as soon as the DOM has loaded and can make the page appear as if it is loading faster.

**Getting Element Content**

![getting content](../img/getting-content)

**Updating Elements**

![updating elements](../img/updating-elements)

**Inserting Elements**

![Inserting elements](../img/inserting-elements)

**Getting And Setting Attribute Values**

![Attributes](../img/set-attr)

**Event Methods**

The `.on()` method is used to handle all events. 

```JavaScript
$('li').on('click', function(){
  $(this).addClass('complete');
});
```

![Events](../img/events)

[Back to Homepage](https://ashcaz.github.io/reading-notes)