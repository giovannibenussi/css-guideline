This is a guideline to design scalable and maintainable sass files.

# Rule Declaration Anatomy

The basic anatomy of a rule declaration is as follows:

```css
.my-class
    // Font related style
    // General element style

    // Margin related style
    // Padding related style
```

Each section should be separated visually by a newline.

For example, if we want a red box with a white font with a font-weight of 300  and 20px of margin and padding we should write something like this:

```css
// Bad
.red-box
    margin: 20px
    padding: 20px
    color: white
    font-weight: 300
    background: red

// Good
.red-box
    color: white
    font-weight: 300

    background: red

    margin: 20px

    padding: 20px
```
