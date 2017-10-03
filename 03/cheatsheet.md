# HTML Cheatsheet

## Tag Anatomy 

`<name attribute="value id="nameID" class="someClass"></name>`

Common attributes:

- id: A unique identifier for a tag. An id must be unique per page (e.g. `main-button`)
- class: a non-unique identifier for a tag (e.g. `blog-post`)

## Main Tags
`<html>` - Defines an HTML document 

`<head>` - Where information about the current page is kept

`<body>` - Where rendered content is kept

## Layout Tags

`<div>` - Creates a "division" not to be confused with `<section>`

## Typeography Tags

`<h1> , <h2>, <h3>, <h4>, <h5>, <h6>` - Heading tags. These render the text designated for section titles 

`<p>` - Creates a paragraph of text

`<span>` - Similar to `<p>` but does not create a line break 

## Media Tags

`<img src="http://someimage.com" />` - Creates an image 

`<video src="http://someVideo.com" />` - Creates a video 

these tags are self closing. They don't require a closing tag but instead of `>` on the right it becomes `/>`

## Creating Links 

Anchor tag: 

`<a href="http://someUrl.com">` 

Wrapping content inside an `<a>` tag makes that element clickable by default. When the item is clicked the page navigates to the `href`.

