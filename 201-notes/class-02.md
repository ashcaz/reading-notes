## Duckett HTML Ch. 2 Text (p.40-61)

**Headings**

- HTM has 6 levels of heading h1-h6
  - `<h1>` is used for main headings 
  - `<h2>` is used for subheadings 
  - ...

**Paragraphs**

- `<p>` tag : To create a paragrah you surround the words that make up a paragraph with a opening `<p>` tag and closing `</p>` tag
- by default when using this tag the browser wil show each paragraph on a new line

**Bold and ***Italic*****

- Tp make a word appear **bold** wrap the word in `<b>` bold `</b>` tags.

- To make a word appear ***italic*** wrap the word in `<i>` italic `</i>` tags.


- **Semantic Markup** does not affect the structure of the webpage but add extra information for things like accesibility functions

## Duckett HTML Ch. 10 Introducing CSS

**Understanding CSS**

- The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.
- CSS allows you to create rules that determines what each individual box is presented
- CSS associates the rules you create with the HTML element. A CSS rule has two parts a **selector** - indicates which element the rule applies to, and a **declaration** -indicates how the elements referred to in the selector should be styled

```javascript
p (selector){
    font-family (property); Arial (value); (everything inside curly brackets = declaration)
}
```

- Declarations sit inside of curly brackets
- Declarations are made up of two parts: a **property** - indicates the aspect of the element you want to change, and a **value** - specify settings you want to use for the chosen property.
- Several properties in one declaration can be specified when separated by a semi-colon

**Using External CSS**

- You can use the link element in an HTML document to tell the browser where to find the CSS file used to style the page

```javascript
link href="css/styles.css" type="text/css" rel="stylesheet"
```

- href specifies the path to the CSS file
- The type attribute  tells you the type of document
- rel specifies the relationship between the HTML page and the file it is linked to

**Using Internal CSS**

- you can style within the HTML document using the style element

**CSS Selectors**

- universal selector :  *{}
- type selector :  h1, h2, h3 {}
- class selector : .note {} or p.note - targets on p elements with that class attribute
- ID selector : #introduction {}
- Child selector : li>a {} - targets any a elements that are children of li
- adjacent sibling selector : h1+p {} - targets first element after any h1 element but no other p element

CSS works in cascading rules - goes from top to bottom, if two rules are identical for one selector the latter of the two with take precedence over the first

**Advantages of External Style Sheet**

- All your web pages can share the same style sheet
- When making a change to all h1 elements you dont have to individually change every element. You only need to change one css style sheet.


## Duckett JS Ch.2 Basic JavaScript Instructions (p.53-84)

**Statements**

- A script is a series of instructions taht a computer can follow one-by-one. (Like a recipe)
- statements end with a semicolon example 
```javascript
var age = 17;
```
- each statement starts on a new line

**Comments**

- Use comments to explain what your code does
```javascript
/* Use this to comment out milti-line comments*/
```
  - Use two forward slashes to do single line comments
  ```javascript
  // Like this
  ``` 
  


**Variables** 

- Variables are used by scripts to temporarily store information
- Before you can use a variable you need to announce that you want to use it
- In order to use a variable you have to give it a name, which is sometimes called an identifier

```javascript 
var = variable keyword
```
```javascript
var quantity;
```

- If varable name is more than one word its usually written in **camelCase**
- Once you've created a variable, you can tell it what information you would like it to store for you aka assigning a value

```javascript
quantity = variable name
```

```javascript
    quantity = 3
```

- Equal sign is the assignment operator it says that you're going to assign a value to the variable
- 3 is the variable value. Until you assign a value the value is undefined

**Data Types**

- The different data types consist of:
  - Numeric data types
  - String data types ('Hi, Ashley!')
  - Boolean data types (True or False)
- There are more data types dicussed in later chapters.

**Rules for naming Variables**

1. Name must begin with a letter
2. Name can contain letters, numbers, dollar sign($) or an underscore (_). No dashes (-)or periods (.)
3. You can not use Keywords or reserved words.
4. All variables are case sensitve. `Score` and `score` are two different variable names.
5. Use a name that describes what information the variable is storing. For example if the variable is storing someones age name the variable age.
6. If your variable is made up of more than one 

## Duckett JS Ch. 4 Decisions & Loops (p.145-162)

**Evaluating Conditions & Conditional Statements**

- There are two componets to a decision:
  1. An expression is evaluated, which returns a value
  2. A conditional statement says what to do in a given situation

```javascript
if (score > 50){
    document.write("You Passed!");
  else {
      document.write("Try again..");
    }
}
```

## Comparison Operators: Evaluating Conditions

You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a **boolean: true or false**

- ```==``` Is equal to
- ```===``` strict equal to
- ```!= ```is not equal to
- ```!==``` strict not equal to
- ```>``` greater than
- ```<``` less than
- ```>=``` greater than or equal to
- ```<=``` lessthan or equal to
- ```&& ```Logical and
- ```||``` Logical or
- ```!``` Logical not

[Back to Homepage](https://ashcaz.github.io/reading-notes)