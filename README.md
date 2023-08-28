# A Basic Introduction to JavaScript and Mouse Events

Once you are comfortable with referencing different elements in the HTML document using the DOM (Document Object Model), the next step is to connect the manipulation of the elements in teh DOM to events. JavaScript has many events that can be connected to blocks of code:

1. onclick
2. ondblclick
3. onmousedown
4. onmousemove
5. onmouseout
6. onmouseover

## Example Event

If we had the following HTML document:

```html
<!doctype html>
<html>
<head>
    <title>The JavaScript DOM</title>
</head>
<body>

  <h1 id="heading">The JavaScript DOM</h1>

  <p id="paragraph">Mauris convallis dictum odio. Quisque euismod finibus.</p>

  <a id="link" href="https://codeadam.ca">codeadam.ca</a>
  
  <button id="button">Click Me!</button>
    
</body>
</html>
```

If we wanted to change the colour of the `h1` element when the `button` element is clicked, we would first create a reference to the button element:

```javascript
var button = document.getElementById('button');
```

And then add an event listener:

```javascript
button.addEventListener("click",function(){
  document.getElementById("heading").styles.color = "red";
});
```

## Trying It Out

Create a new HTML document, add four `div` elements. Add the following four events and DOM manipulation:

1. Change the `background-colour` of the first `div` elements is clicked.
2. Change the `background-colour` of the second `div` element when the mouse enters.
3. Change the `background-colour` of the third `div` element when the mouse leaves.
4. Change the `background-colour` of the fourth `div` element when double clicked.

> Full tutorial URL:  
> https://codeadam.ca/learning/javascript-mouse-events.html

***

## Repo Resources

* [Visual Studio Code](https://code.visualstudio.com/) or [Brackets](http://brackets.io/) (or any code editor)

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
