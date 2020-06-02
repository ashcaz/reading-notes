## Duckett HTML Ch. 7 Forms (p.144-175)

**Form Controls**

- Adding Text
  - Text imput (email address or names)
  - Password input
  - Text area(messages or comments)

- Making choices
  - Radio buttons
  - Checkboxes
  - Drop-down boxes

- Submitting Forms
  - submit buttons
  - image buttons

- Uploading files
  - file uplaod (text box with browse and upload buttons)

**How Forms Work**

1. A user fills in a form and then presses a button to submit the information to the server.

2. The name of each form control is sent to the server along with the value the user enters or selects.

3. The server processes the information using a progamming language such as PHP, C#, vb.net or java. It may also store the information in a database.

4. The server creates a new page to send back to the browser based on the information received

**Form Structure**

- Form controls live inside the `<form>` element

- This elemsnt should always carry the action attribute and will usuually have a method and id attribute too.

- the action attributes value is the  URL for the page on the server that will receive the information in the form when it is submitted.

- Forms can be sent using one of two methods: get or post
  - get method: the values  form the form are added to the URL specified in the action attribute.
    - get method is ideal for short forms or when you are just retrieving data from the web server

  - Post method:values are sent in what are known as HTTP headers. Use when
    - users upload a file
    - form is very long
    - contains sensitive data
    - adds information to , or deletes information from  a database

- If the method attribute is not used get method is the default.

**Text input**

- The `<input>` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.
  - `type="text"` cretes a single line text input
  - `name` disinguishes which form control each piece of data was entered into.
  - `size` should not be used in new forms
  - `maxlength` used to limit the number of characters a user may enter into a field

**Password input**

- `type="password"` creates a text box that acts like a single line input, except the characters are blocked out

## Duckett HTML Ch. 14 Lists, Tables & Forms (p.330-357)

- Lots of CSS notes read book again


## Duckett JS Ch. 6 Events (p.243-292)

- When you browse the web , your browser registers different types of events. Its the browser's way of saying, "hey this happened". Your script can respond to these events
  - Interactions create events
  - Events trigger code
  - Code responds tp users

**Different Types of events**

- `load`
- `error`
- `scroll`
- `click`
- `mouseover`

**How Events Trigger JavaScript Code**

1. Select element node(s) you want the script to respond to.
2. Indicate which event on the selected node(s) will trigger the respose
3. State the code you want to run when the event occurs

**Three Ways To Bind An Event To An Element**

1. HTML Event Handlers
  - THIS IS BAD PROCTICE DO NOT USE

2. Traditional DOM Event Handlers
  
3. DOM level 2 Event Listeners


[Back to Homepage](https://ashcaz.github.io/reading-notes)