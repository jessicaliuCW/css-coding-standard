# css-coding-standard

## 命名規格

Always use hyphens in class names. Do not use underscores or CamelCase notation.

```css
/* Correct */
.sec-nav

/* Wrong */
.sec_nav
.SecNav
```

## 值的寫法

Always define generic font families like sans-serif or serif.
```css
/* Correct */
font-family: "ff-din-web-1", Arial, Helvetica, sans-serif;

/* Wrong */
font-family: "ff-din-web-1";
Shorten hexidecimal color values to 3 digits when possible:
background: #fff;
```
## Do not use unit with 0.

```css
/* Correct */
.nav a {
  padding: 5px 0 5px 2px;
}

/* Wrong */
.nav a {
  padding: 5px 0px 5px 2px;
}
```
Do not use default values if they are not necessary to override inherited values.

## 選擇器

Selectors should be on a single line, with a space after the selector, followed by an opening brace. A selector should end with a closing brace on the next line. Next selector related the the previous one should be on the next line with one additional line space between them.
```css
.nav li {
}
 
.nav a {
}
```

Avoid very complex child and descendant selectors like:
```css
/* Wrong */
.my-inbox .flyout-content .inner .message .inbox li div.take-action .actions ul li a {
}
```
## 多項選擇器

Multiple selectors should each be on a single line, with no space after each comma.
```css
.faqs a.open,
.faqs a.close {
}
```
## 屬性

Every declaration should be on its own line below the opening brace. Each property should:

have a single sof tab with 2 spaces before the property name and a single space before the property value.
end in a semi-colon.
```css
.site-name span {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 10;
}
```
## Shorthand properties

Use shorthand properties when possible.

## Order of properties

Order of properties can have the following structure: box model, typography and graphic layer or order properties alphabetically.


## 註解

Follow the comments style used in normalize.css. The comments blocks should be maximum of 80 characters wide.

This comment style is used as the separator of the main sections. There are 2 empty lines before and after it:
```css
/* ==========================================================================
   Section comment block
   ========================================================================== */
The following comment style is used as the separator of the subsections of the main sections. It has 2 empty lines before it and 1 empty line after it:

/* Sub-section comment block
   ========================================================================== */
This comment style is used for commenting particular page elements. It has 1 empty line before it and no empty lines after it (it is immediately followed by the rules):

/* Pager */
.pager {
  padding-bottom: 5px;
  border-bottom: 1px solid #ccc;
}
Use upper case for the first letter in comments:

/* Correct */

/* Pager */

/* Wrong */

/* pager */
```
