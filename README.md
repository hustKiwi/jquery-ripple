jQuery-ripple
=============

A jQuery Plugin for a ripple effect inspired by Google Material Design.

### Installation

jQuery-ripple can be installed through [Bower](http://bower.io/).

    $ bower install jquery.ripple --save

Or through [npm](https://docs.npmjs.com/)
    
    $ npm install jquery-ripple --save

### Usage

1. Include the required jquery.ripple.css in the head section of your document.

    ```
    <link rel="stylesheet" href="bower_components/jquery-ripple/jquery.ripple.css">
    ```
2. Include the latest version of jQuery and jQuery-ripple in your document.

    ```
    <script src="//code.jquery.com/jquery-latest.min.js"></script>
    <script src="bower_components/jquery-ripple/jquery.ripple.js"></script>
    ```
3. Create an element with the `[data-ripple]` data attribute defined.

    ```
    <button data-ripple>Button</button>
    ```
4. Call the plugin on the element.

    ```
    $('[data-ripple]').ripple();
    ```

### Customization

Optionally, you can pass a different CSS color to use for the ripple ink:

```
$('[data-ripple]').ripple({ color: '#EF5734' });
```

### Events

jQuery-ripple introduces three events that you can hook into for additional functionality:

| Event Name | Description |
|----------------|-----------------------------------------------------------------------------------------------------|
| *'beforeripple'* | Fired on touchstart/mousedown before ripple-active class is added to the DOM |
| *'afterripple'* | Fired on touchend/mouseup/mouseleave before ripple-active class is removed from the DOM |
