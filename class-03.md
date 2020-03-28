## Duckett HTML Ch.3 Lists (p.62-73)

**Ordered Lists**

- Ordered lists are created with the `<ol>` tag
- Each item in the list is placed between the opening `<li>` and a closing `<li>` tags.
- Ordered lists show up as a number list

**Unordered Lists**

- Unordered lists are created with a `<ul>` element.
- Each item, like an ordered list, is placed between an opening `<li>` tag and closing `<li>` tag.
- Unodered lists show up as bullet points

## Duckett HTML Ch.13 Boxes (p.300-329)

**Box Dimensions**

- You can use height and width properties in CSS to set your own dimensions for a box.
- You can use pixels, percentage or ems.
  - Pixels sre the most popular
  - When you use percentages, the sixe of the box is relative to the sixe of the browser
  - When using ems, the size of the box is based on the size of the text within it.

**Boarder, Margin & Padding**

- Every box has three available properties that can be adjusted to control its appearance; Boarder, margin and padding.
  1. Boarder
    - Every box has a boarder even if its not visable.
    - The boarder seperates the edge of one box from another.
    - Boarder-width, boarder-style and boarder-color properties are popular(p.310)
  2. Margin
    - Margins sit outside of the edge of the boarder
    - you can set the width of the margin to create a gap between the boarder of two adjacent boaxes
  3. Padding
    - Padding is the space between teh boarder of the box and any content contained within it.
    - Adding padding can increase readability of its contents

    **Change Inline/Block**

    - The `display` property allows you to turn an inline element into a block level element or vice versa.
      - Values
        - inline: causes a block-level element to act like an inline element
        - block: causes and inline element to act like a block-level element 
        - inline-block: cause a block level element to flow like an inline element, while retaining other features fo a block-level element
        - none: this hides an element form the page
        
## Duckett JS Chapter 4: Decisions and loops (p.162-182)

**Switch Statements**

- A switch statement starts with a variable called the **switch value**. each case indicates a possible value for this variable and the code that should run if the variable matches that value.

- Switch statements differ from if-else statements:

  - If you have a deafault option thatt is run if none of the cause match
  - If a match is found, that code is run; then the break statement stops the rest of the switch statement running
  - better then mulitiple if statements

**Loops**

- Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true the code block will run again. It repeats until the condition returns false.

for(var i = 0; i < 10; i++){
    document.write(i);
}

**For Loops** 
 
 - A for loop is often used to loop through the items in an array.
 
**While Loop**

- This loop continues to run for as long as the condition in the parentheses is true.

**Do While loops**

- The key difference between a while loop and a do while loop is that the statements in the code block come before the condition. This means that those statements are run once wether or not the condition is met.

[Back to Homepage](https://ashcaz.github.io/reading-notes)