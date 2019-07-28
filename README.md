# CSS ANIMATIONS
Animations using only CSS + JS when needed

## CSS +  HTML only Bubbles
An alternative to the Bubbles sample at: https://www.creativebloq.com/inspiration/css-animation-examples <br />
This one has added support to IE11 and yes, it is responsive too  

To have the correct spacing calculation, consider to use Scss, something like:
```Scss
$width: 500px;
$limit: 9;

@for $i from 1 to 10 {
  .bubb-sm-#{$i + 1}{
    /*IE Support*/
    transform: translateX(ceil($width * ($i/$limit) - 11px));
    
  }
}

```

### Demo
See the working sample at: https://accedo-gps.000webhostapp.com/demo/css-bubbles/index.html

## CSS + HTML + SVG Bubbles
This option uses SVG, the downside with SVG, the CSS properties *transform* are not supported at all in IE11 but you can change them and add them as attributes to the SVG element directly.

### Demo
See a working demo using these choices at: https://accedo-gps.000webhostapp.com/demo/css-bubbles/svg-bubbles.html
