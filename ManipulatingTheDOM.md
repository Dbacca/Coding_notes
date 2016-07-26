# Manipulating the DOM


JQuery allows us to create new elements like the `<p>` below and insert them into the page.

###### Common methods of appending to the DOM include:

`.appendTo(<element>)`
`.prependTo(<element>)`
`.insertAfter(<element>)`
`.insertBefore(<element>)`

##### Example

``` javascript
function(){
var price = $("<p> From $399</p>")
// creates a paragraph element with the price
  $(".car").append(price);
    //add the paragraph
  $("button").remove();
    // hide the button
```

### Watching for click
jquery allows you to watch for actions on certain elements within your page. Things like `click` `hover` `keyUp` can be used to trigger a javascript action.

#### Example
``` javascript
  $('button').on('click',function(){
    console.log("you clicked a button")
  //run this function on click
  });
```
