This is a guideline to design scalable and maintainable sass files.

# Rule Declaration Anatomy

The basic anatomy of a rule declaration is as follows:

```css
.my-class
    // Font related style

    // General element style

    // Padding related style
```

Each section should be separated visually by a newline.

For example, if we want a red box with a white font with a font-weight of 300  and 20px of padding we should write something like this:

```css
// Bad
.red-box
    padding-left: 20px
    padding-right: 30px
    color: white
    font-weight: 300
    background: red

// Good
.red-box
    color: white
    font-weight: 300

    background: red

    padding-left: 20px
    padding-right: 30px
```

## Font and general rule organization
In the font and general rule declaration, you should organize the properties in alphabetical order:

```css
// Bad
font-size: 14px
color: white
font-weight: 300
font-style: italic

// Good
color: white
font-size: 14px
font-style: italic
font-weight: 300
```

## Margin and padding rule organization
When you declare a margin or padding rule, you should follow the order botton-top-left-right as follows (the same for margin):

```css
padding
padding-bottom
padding-top
padding-left
padding-right
```
