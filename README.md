# css-animations
Animations using only CSS + JS when needed

## CSS Bubbles
An alternative to the Bubbles sample at: https://www.creativebloq.com/inspiration/css-animation-examples <br />
This one has added support to IE11 and yes, it is responsive too  

To have the correct spacing calculation, consider to use Sass, something like:
```
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
