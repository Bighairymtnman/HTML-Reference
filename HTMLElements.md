# HTML Elements Guide

## Basic Elements
- `<html>`: The root element that contains all other elements
- `<head>`: Contains page metadata and links to external files
- `<body>`: Contains all visible page content
- `<title>`: Sets the page title in browser tab

## Text Elements
- `<h1>` to `<h6>`: Headings (largest to smallest)
- `<p>`: Paragraph of text
- `<br>`: Line break
- `<strong>`: Bold text
- `<em>`: Italic text
- `<span>`: Inline text container

## Lists
- `<ul>`: Unordered (bullet) list
- `<ol>`: Ordered (numbered) list
- `<li>`: List item

## Links & Images
- `<a>`: Creates links to other pages or resources
- `<img>`: Displays images
- `<figure>`: Container for images with captions
- `<figcaption>`: Caption for an image

## Basic Form Elements
- `<form>`: Container for form elements
- `<input>`: Creates various input fields
- `<label>`: Labels for form inputs
- `<button>`: Clickable button
- `<select>`: Dropdown menu
- `<option>`: Items in a dropdown menu
- `<textarea>`: Multi-line text input

## Common Containers
- `<div>`: Generic block container
- `<header>`: Page or section header
- `<nav>`: Navigation links
- `<main>`: Main content area
- `<footer>`: Page or section footer






## Common Page Structure Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>My Blog Post</title>
</head>
<body>
    <!-- Header with navigation -->
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main content area -->
    <main>
        <article>
            <h1>Welcome to My Blog</h1>
            
            <figure>
                <img src="blog-image.jpg" alt="Blog topic image">
                <figcaption>Image describing our topic</figcaption>
            </figure>

            <p>This is the main content of my blog post. It includes <strong>important text</strong> 
            and <em>emphasized points</em>.</p>

            <h2>Key Points</h2>
            <ul>
                <li>First important point</li>
                <li>Second important point</li>
                <li>Third important point</li>
            </ul>

            <!-- Comment form -->
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name">

                <label for="comment">Comment:</label>
                <textarea id="comment" name="comment"></textarea>

                <button type="submit">Submit Comment</button>
            </form>
        </article>
    </main>

    <footer>
        <p>&copy; 2025 My Blog. All rights reserved.</p>
    </footer>
</body>
</html>
```
