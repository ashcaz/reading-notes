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








[Back to Homepage](https://ashcaz.github.io/reading-notes)