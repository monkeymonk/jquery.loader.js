jQuery.loader Plugin - v 1.0
==================

Display a loader on your page or HTML block element.

Project site: http://monkeymonk.github.com/jquery.loader.js/

Demo: http://monkeymonk.be/jquery.loader.js/demo/


## Usage

### Basic

First of all, include `jquery.loader.js (1.526 kb)`, `jquery.loader.min.css (1.135 kb)` and `loader.gif (3.866 kb)` in your HTML then start to use jQuery.loader.

``` javascript
$(document).ready(function() {
    $('body').loader('show');

    setTimeout(function () {

        $('body').loader('hide');

    }, 2000);
});
```

### Options

``` javascript
{
    className: 'loader',

    tpl: '<div class="{className} hide"><div class="{className}-load"></div><div class="{className}-overlay"></div></div>',

    delay: 200,
    loader: true,       // if true, you can hide the loader by clicking on it
    overlay: true,      // display or not the overlay

    // Callback
    onHide: function () {},
    onShow: function () {}
}
```

### Methods

#### jQuery().loader('show', options);

jQuery.loader use a tiny template system that let you an easy way to customize your loader.

``` javascript
$('body').load('show', {
    onHide: function () {
        // do something...
    }
});

```

#### jQuery().loader('hide', onHide);

Hide the loader

``` javascript
$('body').loader('hide');

```



## Browsers: Tested and Working In

- IE 6, 7, 8, 9, 10
- Firefox 3+
- Opera 10+
- Safari 4+

