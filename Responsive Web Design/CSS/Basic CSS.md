# Change The Colour of A Text
### Inline-CSS
Edit **color** property of **style** via inline-CSS. End the inline with `;`.
`<h2 style="color: blue;">CatPhotoApp</h2>`

### Style Blocks
Instead of styling elements individually via inline CSS, it's better to use style blocks. The code below makes all **h2** elements red.
 ```
<style>
  h2 {
    color: red;
  }
</style>
```

### Using Classes to Style Elements
```
<style>
  .blue-text {
    color: blue;
  }
</style>
```

# Change The Font Size of An Element
Font size of an element is controlled by `font-size` property of CSS.
```
<style>
  h1 {
    font-size: 30px;
  }
</style>
```

# Set the Font Family of an Element
`font-family` property of CSS determines which font will be used by an element. 
```
<style>
  p {
    font-family: monospace;
  }
</style>
```

# Import Google Fonts
Import a font from https://fonts.google.com/, then use it via `font-family` property. If the font name includes any whitespaces, make sure you wrap the font name inside double quotes.
In this example, Lato font is imported, and monospace is also called in case Lato cannot be found.
```
<link href='http://fonts.googleapis.com/css?family=Lato&subset=latin,latin-ext' rel='stylesheet' type='text/css'>
<style>
  p {
    font-family: Lato, monospace;
  }
</style>
```
# Image Sizing
```
<style>
  .menu-image {
    width: 50px;
  }
</style>
```

# Multiple Classes
`<img class="class1 class2" src="https://....">`

# CSS Borders
```
.thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 10px;
  }
```
For circular images: `border-radius: 50%;`

# Background Colour
```
.green-background {
  background-color: green;
}
```

# ID vs Class
The only difference between them is that “id” is unique in a page and can only apply to at most one element, while “class” selector can apply to multiple elements. ID has a higher importance over class selectors.
```
<style>
 #cover {
 }
 
 .coverimg{
 }
</style>
.
.
<img id="cover" class="coverimg" src="...." alt="....">
```
# Padding & Margin
**Padding** controls the space between the content and its border. 
**Margin** controls the space between its border and the outer/surrounding elements.
```
  .red-box {
    background-color: crimson;
    color: #fff;
    padding: 20px;
    margin-top: 40px;
    margin-left: 40px;
    margin-right: 20px;
    margin-bottom: 20px;
  }
  }

  .blue-box {
    background-color: blue;
    color: #fff;
    padding-top: 40px;
    padding-left: 40px;
    padding-bottom: 20px;
    padding-right: 20px;
    // padding: 40px 20px 20px 40px; clockwise notation from top-right-bottom-left
  }
```

# Attribute Selectors
Select elements by their attributes and corresponding values.

```
[type='button'] {
    margin: 10px;
    padding: 1.5em; //relative property
}
```
# The Override in Subsequent CSS Classes
- The second declaration will always take precedence over the first in **style** blocks.
- ID attributes always take precedence over Class attributes in **style** blocks.
- Inline CSS styling is applied rather than **style** blocks.
- The last and most powerful way to make sure that a CSS is absolutely applied, use `!important` keyword.
```
<style>
  body {
    background-color: black;
    font-family: monospace;
    color: green;
  }
  #orange-text {
    color: orange;
  }
  .pink-text {
    color: pink !important; //no matter what other overrides are, this is the highest priority
  }
  .blue-text {
    color: blue;
  }
</style>
<h1 id="orange-text" class="pink-text blue-text" style="color: white;">Hello World!</h1>
```

