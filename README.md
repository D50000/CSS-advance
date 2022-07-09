# CSS Advance

Here will note the important concept and advance skill.

## CSS Specificity

Definition of applying the style selector by priorities. The element will apply the highest Specificity's style.

```html
<html>
  <head>
    <style>
      #demo {
        color: blue;
      }
      .test {
        color: green;
      }
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <p id="demo" class="test" style="color: pink;">Hello World!</p>
  </body>
</html>
```

- High Specificity

1. inline style
2. #id
3. class style
4. html tag style

## Special Symbols CSS Selector

https://techbrij.com/css-selector-adjacent-child-sibling
https://css-tricks.com/useful-nth-child-recipies/

### Reference

- https://www.w3schools.com/css/css_specificity.asp
