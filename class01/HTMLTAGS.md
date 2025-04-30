# HTML Tags - Class Notes

## Basic Structure Tags
```html
<!DOCTYPE html> <!-- Defines document type and HTML version -->
<html> <!-- Root element of HTML document -->
<head> <!-- Contains meta information about the document -->
<title>Page Title</title> <!-- Specifies the title displayed in browser tab -->
</head>
<body> <!-- Contains the visible page content -->
</body>
</html>
```

## Heading Tags
```html
<h1>Most Important Heading</h1>
<h2>Subheading</h2>
<h3>Third-level heading</h3>
<h4>Fourth-level heading</h4>
<h5>Fifth-level heading</h5>
<h6>Least Important Heading</h6>
```

## Text Formatting Tags
```html
<p>This is a paragraph.</p>
<b>Bold text</b>
<strong>Important text (semantic bold)</strong>
<i>Italic text</i>
<em>Emphasized text (semantic italic)</em>
<mark>Highlighted text</mark>
<small>Smaller text</small>
<del>Deleted text</del>
<ins>Inserted text</ins>
<sub>Subscript</sub>
<sup>Superscript</sup>
```

## Link and Image Tags
```html
<a href="https://example.com">Link text</a>
<img src="image.jpg" alt="Description" width="200" height="100">
```

## List Tags
```html
<ul> <!-- Unordered list -->
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<ol> <!-- Ordered list -->
  <li>First item</li>
  <li>Second item</li>
</ol>

<dl> <!-- Description list -->
  <dt>Term</dt>
  <dd>Definition</dd>
</dl>
```

## Table Tags
```html
<table>
  <tr> <!-- Table row -->
    <th>Header 1</th> <!-- Table header -->
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td> <!-- Table data -->
    <td>Data 2</td>
  </tr>
</table>
```

## Form Tags
```html
<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label>
  
  <input type="checkbox" id="subscribe" name="subscribe">
  <label for="subscribe">Subscribe</label>
  
  <select name="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </select>
  
  <textarea name="message" rows="4" cols="30"></textarea>
  
  <button type="submit">Submit</button>
</form>
```

## Semantic Tags (HTML5)
```html
<header>Header content</header>
<nav>Navigation links</nav>
<main>Main content</main>
<section>Section of content</section>
<article>Independent, self-contained content</article>
<aside>Sidebar content</aside>
<footer>Footer content</footer>
```

## Media Tags
```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
</audio>

<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
</video>

<iframe src="https://example.com"></iframe>
```

## Other Important Tags
```html
<div>Block-level container</div>
<span>Inline container</span>
<br> <!-- Line break -->
<hr> <!-- Horizontal rule -->
<!-- This is a comment -->
<code>Computer code</code>
<pre>Preformatted text</pre>
```

## Meta Tags (in head section)
```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```