A guideline to design scalable and maintainable stylesheets.

# Table of contents
* [Introduction](https://giovannibenussi.github.io/sass-style-guide/#introduction)
* [Doctrine](https://giovannibenussi.github.io/sass-style-guide/#doctrine)
* [Rule Declaration Anatomy
](https://giovannibenussi.github.io/sass-style-guide/#rule-declaration-anatomy)
* [Font and general rule organization](https://giovannibenussi.github.io/sass-style-guide/#font-and-general-rule-organization)
* [Margin and padding rule organization](https://giovannibenussi.github.io/sass-style-guide/#margin-and-padding-rule-organization)

# Introduction
This is a guideline written with the purpose of have a common coding style and conventions, thus allowing developers to rapid and easily find where they should make certain changes. It's simple, if you and your team follow this recommendations, all of you will benefit from a reduced amount of time required in finding the code that modifies some element and the time spent knowing where modify certain properties (color, font-type, padding, etc).

# Doctrine
- Never use _id selectors_
- Never include position related rules inside a component definition (margin, position, etc), because they will make your component not reusable

# Rule Declaration Anatomy

The basic anatomy of a rule declaration is as follows:

```css
.my-class {
    // Font related style

    // General element style

    // Padding related style
}
```

Each section should be separated visually by a newline.

For example, if we want a red box with a white font with a font-weight of 300  and 20px of padding we should write something like this:

```css
// Bad
.red-box {
    padding-left: 20px
    padding-right: 30px
    color: white
    font-weight: 300
    background: red
}
// Good
.red-box {
    color: white
    font-weight: 300

    background: red

    padding-left: 20px
    padding-right: 30px
}
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
