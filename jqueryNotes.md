Jquery Notes!
===

DOM interface is slightly different in all broswers.

Jquery allows you to use communicate across all modern browsers.

### Locate elements using
``` javascript
$('h1').text()
```

### modify text in the H1

``` javascript
 $('h1').text('hello w world')
 ```

### Document Ready function
``` javascript
 $(document.ready(function(){
  <code here>
  }))
  ```
### Target elements by id

``` javascript
 $("#destinations")
 ```

### Target elements by class
``` javascript
$(".articles")
```
## Searching the DOM

### Select *ALL* the ``li`` element with in ``#destinations``
``` javascript
$("#destinations li")
```
### Select *ONLY* the *direct* children
``` javascript
$("#destinations > li")
```

## Selecting *multiple* elements using a coma
``$(".promo, #france")``

### CSS-like pseudo classes
``` javascript
$("#destinations li:first");
$("#destinations li:last" );
$("#destinations li:odd");
$("#destinations li:even");
```

### Traversing the DOM

``` javascript
$(#destinations).find("li");
```
### Using `first()`
This selects the first `li`
``` javascript
$("li").first();
```
### Using `last()`
This selects the last `li`.
``` javascript
 $(".vacation").last();
```
### Using `prev()`
This is used to navigate to the previous element. It is added on after `.last()` so it will select the previous `li` element.
``` javascript
$("#vacations li").last().prev();
```
### Traversing up using `parent()`
``` javascript
$(".class").parent("li");
```

### Traversing down using `children()`
this selects all children `li` of the selected `#id`
``` javascript
$("#id").children("li");
