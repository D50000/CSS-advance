# CSS Advance

Here will note the important concept and advance skill of css.

## CSS Specificity

Definition of applying the style selector by priorities. The element will apply the highest Specificity's style.

```html
<html>
  <head>
    <style>
      /* #2 IDs */
      #demo {
        color: blue;
      }
      /* #3 Classes */
      .test {
        color: green;
      }
      /* #4 html element */
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <!-- #1 inline -->
    <p id="demo" class="test" style="color: pink;">Hello World!</p>
  </body>
</html>
```

**Level of Specificity**

1. **Inline style**
2. **#id**
3. **Classes style, pseudo-classes, attribute selectors** Example: .test, :hover, [href]
4. **HTML tag style**

## Special Symbols CSS Selector


### Reference

- https://www.w3schools.com/css/css_specificity.asp
- https://css-tricks.com/useful-nth-child-recipies/
- https://techbrij.com/css-selector-adjacent-child-sibling
