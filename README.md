# css-animations
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

The above in a Sass/Scss preprocessor will output the following:

```Css
.bubb-sm-2 {
  /*IE Support*/
  transform: translateX(45px);
}

.bubb-sm-3 {
  /*IE Support*/
  transform: translateX(101px);
}

.bubb-sm-4 {
  /*IE Support*/
  transform: translateX(156px);
}

.bubb-sm-5 {
  /*IE Support*/
  transform: translateX(212px);
}

.bubb-sm-6 {
  /*IE Support*/
  transform: translateX(267px);
}

.bubb-sm-7 {
  /*IE Support*/
  transform: translateX(323px);
}

.bubb-sm-8 {
  /*IE Support*/
  transform: translateX(378px);
}

.bubb-sm-9 {
  /*IE Support*/
  transform: translateX(434px);
}

.bubb-sm-10 {
  /*IE Support*/
  transform: translateX(489px);
}
```


### Demo
See the working sample at: https://accedo-gps.000webhostapp.com/demo/css-bubbles/index.html

## CSS + HTML + SVG Bubbles
This option uses SVG, the downside with SVG, the CSS properties *transform* are not supported at all in IE11 but you can change them and add them as attributes to the SVG element directly.

### Demo
See a working demo using these choices at:
