## Duckett JS Ch. 3 Object Literals (p.100-105)

**What Is An Object?**

- Objects group together a set of variables and functions to create a model of something you would recognize from the real world.
- In objects variable and funcions have different names.
  - A variable in an object is called a property. Properites tell us about the object.
  - When a function is part of an object, it is called a method. They represent tasks that are associted with the object. 

```JavaScript
var hotel = {
  name: 'Quay',
  rooms: 40,
  booked: 25,
  gym: true,
  roomTypes: ['twin', 'double', 'suite'],
  checkAvailability: function(){
    return this.rooms - this.booked;
  }
}
```
`name = key , 'Quay' = value`

- properites and methods have a name and a value. In an object that name is called a key
- an object can not have two keys with the same name.

**Accessing an Object**

- you can access the properties or methods of an object using dot notation.
- use the name of the object, followed by a period, then the name of the property or method you want to access.

```JavaScript
var hotelName = hotel.name;
var roomFree = hotel.checkAvailabilty;
```

## Duckett Ch. 5 Document Object Model (p.183-242)

- The **Document Object Model** specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

**Caching DOM Queries**

- Methods that find elements in the DOM tree are called DOM queries.
- If you use a querie more than once, you shoudl use a variable to store the querie.

```JavaScript
var itemOne = getElementById ('one');
```

**Selecting An Element From A Nodelist**

-There are two ways to select an element from a nodelist : The `item()` method and array syntax. Both require the index number of the element you want.

```JavaScript
var firstItem = elements.item(0);
var firstItem = elements[0];
```
**Repeating Actions for an Entire NodeList**

- When you have a NodeList, you can loop through each node in the collection and apple the same staements to each.

```JavaScript
var hotItems = document.querySelectorAll('li.hot');
for ( var i = 0; i < hotItems.length; i++){
  hotelItems[i].className = 'cool';
}
```

- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one
node, it will always return a Nodelist.
- From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
-In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree.

[Back to Homepage](https://ashcaz.github.io/reading-notes)