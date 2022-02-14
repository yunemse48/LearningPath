# DOCTYPE Declaration
Since HTML is an evolving technology, it's always required to tell the browser to use which version of HTML by declaring a DOCTYPE at the top of the page. `html` tags are put right below the DOCTYPE declaration and the rest of the code is wrapped in these `html` tags. `<!DOCTYPE html>` defines HTML5. 
```
<!DOCTYPE html>
<html>
  ...
</html>
```

# `head` & `body` Tags
`head` and `body` tags are defined withing `html` tags to increase organisational level of the page. `head` element includes information of the page like metadata elements, `link`, `meta`, `title`, `style`. The content displayed to users is wrapped inside the `body` element. 
```
<!DOCTYPE html>
<html>
  <head>
    <meta .../>
    ...
  </head>
  <body>
    <div>
    ...
    </div>
  </body>
</html>
```

# Headlines

```
H1 --> <h1>something</h2>
.
.
.
H6 --> <h6>something</h6>
```

# Paragrapgh

`<p>This is a paragraph</p>`

# Main Tag

`<main>...</main>` tag is used to enclose the content for both structure, readability and SEO.

# Image Tag

"Self-enclosing" tags for embedding images...
`<img src="https://example.com/example.png" alt="Example Image Alternate Text">`

# Unordered (Bullet) List
```
<ul>
  <li>paper</li>
  <li>pen</li>
</ul>
```

# Ordered List
```
<ol>
  <li>paper</li>
  <li>pen</li>
</ol>
```

# Text Field
`<input type="text">` => **input** tags are self-closing
`<input type="text" placeholder="Name" required>` => **required** attribute is optional, and it makes this field mandatory to be filled

# Form Element
Web forms submit data to a server by specifying an **action** attribute on the form element.
It might be **absolute** or **relative** path.
```
<form action="/register">
  <input type="text">
</form>
```

# Button
`<button type="submit">Submit</button>`

# Radio Buttons & Checkboxes
### Radio buttons are used for questions that have only one answer.

Submit *indoor-outdoor=on*
```
<label for="indoor">
  <input id="indoor" type="radio" name="indoor-outdoor">Indoor 
</label>
```
Submit *indoor-outdoor=outdoor*
```
<label for="outdoor"> 
  <input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor">Outdoor 
</label>
```

### Checkboxes are used for questions that can have multiple answers.
```
<label for="honest"><input id="honest" value="honest" type="checkbox" name="personality">Honest</label>
<label for="kind"><input id="kind" value="kind" type="checkbox" name="personality">Kind</label>
<label for="rude"><input id="rude" value="rude" type="checkbox" name="personality">Rude</label>
```
> Selected radio buttons and checkboxes send `on` when submitted in default. However, it's not that useful. Always make sure that you create meaningful `name` and `value` attributes.
> Checkboxes and radio buttons can be checked by default.

`<input type="radio" name="test-name" checked>`

# `div` Elements
The div element, also known as a division element, is a general purpose container for other elements. It's non-self-closing. 
```
<div>
  <p> This is a paragraph.</p>
  <ul>
    <li>Red</li>
    <li>Blue</li>
  </ul>
  <img src="example.png" alt="example">
</div>
```
