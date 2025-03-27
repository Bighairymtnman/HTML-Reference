# HTML Basics Reference

## Document Structure
/* The foundation of every HTML document - this template ensures proper rendering and responsive design */
1. Basic HTML Template
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Page Title</title>
   </head>
   <body>
       <!-- Content goes here -->
   </body>
   </html>
   ```

## Text Elements
/* Headings create document hierarchy and improve SEO */
1. Headings
   ```html
   <h1>Main Heading</h1>      <!-- Use only one h1 per page -->
   <h2>Subheading</h2>        <!-- Major sections -->
   <h3>Section Heading</h3>    <!-- Subsections -->
   <h4>Subsection Heading</h4> <!-- Deeper levels -->
   <h5>Small Heading</h5>      <!-- Rarely used -->
   <h6>Smallest Heading</h6>   <!-- Rarely used -->
   ```

/* Basic text formatting elements for content structure */
2. Paragraphs and Text Formatting
   ```html
   <p>This is a paragraph of text.</p>      <!-- Basic text block -->
   <strong>Bold text</strong>               <!-- Important text -->
   <em>Italic text</em>                     <!-- Emphasized text -->
   <br> <!-- Single line break -->
   <hr> <!-- Horizontal line to separate content -->
   ```

## Lists
/* Three types of lists for organizing content */
1. Unordered List
   ```html
   <ul>                    <!-- For non-sequential items -->
       <li>First item</li>
       <li>Second item</li>
       <li>Third item</li>
   </ul>
   ```

2. Ordered List
   ```html
   <ol>                    <!-- For sequential items -->
       <li>First step</li>
       <li>Second step</li>
       <li>Third step</li>
   </ol>
   ```

3. Description List
   ```html
   <dl>                    <!-- For term-definition pairs -->
       <dt>Term</dt>
       <dd>Definition of the term</dd>
       <dt>Another term</dt>
       <dd>Definition of another term</dd>
   </dl>
   ```

## Links and Images
/* Essential elements for navigation and visual content */
1. Links
   ```html
   <a href="https://www.example.com">External Link</a>     <!-- Links to other websites -->
   <a href="page.html">Internal Link</a>                   <!-- Links within your site -->
   <a href="mailto:email@example.com">Email Link</a>       <!-- Opens email client -->
   <a href="tel:+1234567890">Phone Link</a>               <!-- For phone numbers -->
   ```

2. Images
   ```html
   <img src="image.jpg" alt="Description of image">              <!-- Basic image with alt text -->
   <img src="https://example.com/image.jpg" alt="Online image"> <!-- Remote image -->
   <figure>                                                      <!-- Image with caption -->
       <img src="image.jpg" alt="Figure image">
       <figcaption>Image caption</figcaption>
   </figure>
   ```

## Tables
/* Structured data presentation */
1. Basic Table Structure
   ```html
   <table>                     <!-- Container for tabular data -->
       <thead>                 <!-- Table header section -->
           <tr>               <!-- Table row -->
               <th>Header 1</th>  <!-- Header cell -->
               <th>Header 2</th>
           </tr>
       </thead>
       <tbody>                <!-- Table body section -->
           <tr>
               <td>Data 1</td>    <!-- Data cell -->
               <td>Data 2</td>
           </tr>
       </tbody>
   </table>
   ```

## Forms
/* User input collection elements */
1. Basic Form Structure
   ```html
   <form action="/submit" method="post">     <!-- Container for form elements -->
       <label for="username">Username:</label>
       <input type="text" id="username" name="username">
       
       <label for="password">Password:</label>
       <input type="password" id="password" name="password">
       
       <input type="submit" value="Submit">
   </form>
   ```

2. Common Form Elements
   ```html
   <!-- Various input types for different data collection needs -->
   <input type="text" name="name">          <!-- Single-line text input -->

   <input type="email" name="email">        <!-- Email validation -->

   <input type="checkbox" name="subscribe" id="subscribe">    <!-- Toggle option -->
   <label for="subscribe">Subscribe to newsletter</label>

   <input type="radio" name="gender" value="male" id="male"> <!-- Single choice from group -->
   <label for="male">Male</label>
   <input type="radio" name="gender" value="female" id="female">
   <label for="female">Female</label>

   <select name="country">                  <!-- Dropdown selection -->
       <option value="usa">USA</option>
       <option value="uk">UK</option>
       <option value="canada">Canada</option>
   </select>

   <textarea name="message" rows="4" cols="50"></textarea>    <!-- Multi-line text input -->
   ```

## Semantic Elements
/* Meaningful page structure elements */
1. Page Structure Elements
   ```html
   <header>                    <!-- Top of page or section -->
       <nav>                   <!-- Navigation menu -->
           <ul>
               <li><a href="#home">Home</a></li>
               <li><a href="#about">About</a></li>
           </ul>
       </nav>
   </header>

   <main>                      <!-- Main content area -->
       <article>               <!-- Self-contained content -->
           <h1>Article Title</h1>
           <p>Article content...</p>
       </article>

       <section>               <!-- Thematic grouping -->
           <h2>Section Title</h2>
           <p>Section content...</p>
       </section>

       <aside>                 <!-- Related content -->
           <h3>Sidebar</h3>
           <p>Related content...</p>
       </aside>
   </main>

   <footer>                    <!-- Bottom of page or section -->
       <p>&copy; 2024 Your Website</p>
   </footer>
   ```

## Container Elements
/* Generic containers for layout and styling */
1. Generic Containers
   ```html
   <!-- Division - block-level container for layout -->
   <div class="container">
       <h2>Container Title</h2>
       <p>Container content...</p>
   </div>

   <!-- Span - inline container for text styling -->
   <p>This is <span class="highlight">highlighted</span> text.</p>
   ```

## Meta Tags and SEO
/* Document metadata and search engine optimization */
1. Essential Meta Tags
   ```html
   <head>
       <!-- Character encoding for proper text rendering -->
       <meta charset="UTF-8">
       
       <!-- Mobile responsive settings -->
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       
       <!-- Search engine optimization tags -->
       <meta name="description" content="Page description for search engines">
       <meta name="keywords" content="relevant, keywords, for, page">
       <meta name="author" content="Author Name">
       
       <!-- Social media sharing tags -->
       <meta property="og:title" content="Page Title">
       <meta property="og:description" content="Page description for social media">
       <meta property="og:image" content="image-url.jpg">
       
       <!-- Website icon -->
       <link rel="icon" type="image/x-icon" href="favicon.ico">
       
       <!-- Browser tab title -->
       <title>Your Page Title</title>
   </head>
   ```

