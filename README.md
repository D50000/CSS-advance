# CSS Advance

Here will note the important concept and advance skill of css.

## CSS `Specificity`

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
3. **Classes style, pseudo-classes, attribute selectors** -> Example: .test, :hover, [href]
4. **HTML tag style**

## `:nth` Selector

```css
/* Select first and last li */
li:first-child
li:last-child

/* Select odd and even li */
li:nth-child(odd)
li:nth-child(even)

/* Select fifth li */
li:nth-child(5)

/* Select last second li */
li:nth-last-child(2)

/* Select all li above sixth */
/* Select all li one ~ sixth */
li:nth-child(n+6)
li:nth-child(-n+6)

/* Same as select 4n+1 li */
li:nth-child(4n-7)
```

<img src="https://github.com/D50000/CSS-advanced/blob/master/assets/:nth.jpg" width="400" height="400"/>

## `Special Symbols` Selector

- Have the same parent and immediately `select one` after the first selector.

```css
div + p {
  color: green;
}
```

- Have the same parent and `select all` after the first selector.

```css
div ~ p {
  background-color: blue;
}
```

### Reference

- https://www.w3schools.com/css/css_specificity.asp
- https://github.com/D50000/ob-hover
- https://css-tricks.com/examples/nth-child-tester/
- https://css-tricks.com/useful-nth-child-recipies/
- https://techbrij.com/css-selector-adjacent-child-sibling
