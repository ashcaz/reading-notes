# Django CRUD and Forms

**LINKS**

- [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

- [Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)
- [Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)

## Django Tutorial Part 9: Working with forms

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in `POST` requests with cross-site request forgery protection.

### HTML Forms

The form is defined in HTML as a collection of elements inside form tags, containing at least one input element of type="submit".

```HTML
<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form>
```

[Back to Homepage](https://ashcaz.github.io/reading-notes)
