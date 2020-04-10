## Duckett HTML Ch. 6 Tables (p.126-145)

**What's A Table?**

- A table represents information in a grid format

**Basic Table Structure**

- The `<table>` element is used to create a table
- Contents of the table are written out row by row
- `<tr>` (table row) indicates the start of each row
- its followed by one or more `<td>` (table data)tag. One for each cell in the row.
- at the end of the row use a closing `</tr>` tag.

**Table Headings**

- The `<th>` element is used just like the `<td>` element but its purose is to represent the heading for either a column or a row.

## Duckett JS Ch.3 Functions, Methods and Objects (p.106-144)

**Creating an Object: Constructor Notation**

- the **new** keyword and the object constructor create a blank object. You can then add properties and methods to the object using dot notation.

```javascript
var hotel = new Object();

hotel.name = 'Quay';
hotel.rooms = 40;
hotel.booked = 25;

hotel.checkAvailability = function (){
  return this.rooms -this.booked;
};
```

**Creating Many Objects: Constructor Notation**

- Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects.

```javascript
function Hotel(name, rooms, booked){
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  this.checkAvailability = function(){
    return this.rooms - this.booked;
  };
}
```
- create **instances** of the object usinf the constructer function. The **new** keyword folloed by a call to the function creates a new object. The properties of each are given as arguments to the function.

```javascript
var quayHotel = new Hotel('Quay',40,25);
var parkHotel = new Hotel('Park',120,77);
```

[Back to Homepage](https://ashcaz.github.io/reading-notes)