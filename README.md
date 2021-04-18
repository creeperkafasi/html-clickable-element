# HTML click-element
A javascript library that implements a clickable-element class with onstatechange, onclickstart and onclickend functions.

### Installation & Usage:
* Clone the repository or download the repository as zip.
* Copy the `clickElement.js` file to a directory that you can navigate from your html file.
* Insert the following code ***right before closing your `body` tag***:\
`<script src="/path/to/the/clickElement.js"></script>` (replace `/path/to/the/` with the path to your `clickElement.js` file)
* Usage:
```HTML
<!--HTML-->
<body>
  <clickable-element id="exampleClickable">Click Me</clickable-element>
  
<!--Remember to put the script tag after you finish using the custom elements-->
  <script src="clickElement.js"></script>
</body>
``` 
```CSS
/*CSS*/
#exampleClickable{
  background: blue;
}
#exampleClickable[state="on"]{
  background: red;
}
```
```JS
//Javascript
document.getElementById("exampleClickable").onstatechange = ()=>{
  console.log(document.getElementById("exampleClickable").state)
}
document.getElementById("exampleClickable").onclickstart = ()=>{
  console.log("click start")
}
document.getElementById("exampleClickable").onclickend = ()=>{
  console.log("click end")
}
```
* If you can't see the clickable-element, make sure you followed the steps correctly and make sure your clickable-element has something in it or has a set size (this element behaves like a div by default)

## You can use and modify my code as much as you want!
### Though i would appreciate if you credited me :)
