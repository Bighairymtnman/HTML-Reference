# Advanced HTML Reference

## Advanced Form Controls
/* Modern form elements providing enhanced user interaction and data validation */
1. Advanced Input Types
   ```html
   <!-- Date and time inputs with built-in validation -->
   <input type="date" name="event-date">
   <input type="time" name="meeting-time">
   <input type="datetime-local" name="schedule">
   
   <!-- Numeric inputs with controls -->
   <input type="number" min="0" max="100" step="5">
   <input type="range" min="0" max="100" value="50">
   
   <!-- Color picker -->
   <input type="color" name="theme-color">
   
   <!-- File upload with multiple files and type restrictions -->
   <input type="file" multiple accept="image/*">
   ```

## Interactive Elements
/* Modern HTML elements for user interaction without JavaScript */
1. Details and Summary
   ```html
   <details>
       <summary>Click to expand</summary>
       <p>Hidden content revealed when clicked.</p>
   </details>

   <!-- Nested expandable sections -->
   <details>
       <summary>Main Section</summary>
       <details>
           <summary>Subsection</summary>
           <p>Nested content here.</p>
       </details>
   </details>
   ```








## Advanced Multimedia
/* Modern multimedia elements with enhanced controls and features */
1. Advanced Video Implementation
   ```html
   <video width="720" height="480" controls preload="metadata">
       <source src="video.mp4" type="video/mp4">
       <source src="video.webm" type="video/webm">
       <track src="subtitles.vtt" kind="subtitles" srclang="en" label="English">
       Your browser doesn't support video playback.
   </video>
   ```

2. Advanced Audio Features
   ```html
   <audio controls crossorigin="anonymous">
       <source src="audio.mp3" type="audio/mpeg">
       <source src="audio.ogg" type="audio/ogg">
       <track src="lyrics.vtt" kind="lyrics" srclang="en" label="English">
   </audio>
   ```

## Canvas and SVG
/* Graphics and animation capabilities */
1. Canvas Element
   ```html
   <canvas id="myCanvas" width="500" height="300">
       Your browser doesn't support canvas.
   </canvas>
   ```

2. Inline SVG
   ```html
   <svg width="100" height="100">
       <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red"/>
       <rect x="10" y="10" width="30" height="30" fill="blue"/>
   </svg>
   ```





## Advanced Data Attributes
/* Custom data attributes for storing extra information */
1. Data Attributes Usage
   ```html
   <article
       data-category="technology"
       data-publish-date="2024-01-20"
       data-author-id="123">
       <h2>Article Title</h2>
       <p>Content here...</p>
   </article>

   <button 
       data-action="share"
       data-platform="twitter"
       data-url="https://example.com">
       Share on Twitter
   </button>
   ```

## Advanced Semantic Elements
/* Specialized semantic elements for specific content types */
1. Complex Article Structure
   ```html
   <article>
       <header>
           <h1>Article Title</h1>
           <time datetime="2024-01-20">January 20, 2024</time>
       </header>

       <section>
           <h2>Introduction</h2>
           <p>Opening paragraph...</p>
           
           <figure>
               <picture>
                   <source media="(min-width: 800px)" srcset="large.jpg">
                   <source media="(min-width: 400px)" srcset="medium.jpg">
                   <img src="small.jpg" alt="Responsive image">
               </picture>
               <figcaption>Image description</figcaption>
           </figure>
       </section>

       <footer>
           <address>
               By <a href="mailto:author@example.com">Author Name</a>
           </address>
       </footer>
   </article>
   ```





## Advanced Form Validation
/* Complex form validation and organization techniques */
1. Advanced Form Patterns
   ```html
   <form id="registration" novalidate>
       <!-- Pattern matching for specific formats -->
       <input 
           type="text" 
           pattern="[A-Za-z]{3,}"
           title="Minimum three letters"
           required>

       <!-- Custom validation messages -->
       <input 
           type="email"
           oninvalid="this.setCustomValidity('Please enter a valid email')"
           oninput="this.setCustomValidity('')">

       <!-- Fieldset for grouping -->
       <fieldset>
           <legend>Contact Preferences</legend>
           <input type="checkbox" name="contact[]" value="email">
           <input type="checkbox" name="contact[]" value="phone">
       </fieldset>
   </form>
   ```

## Advanced Metadata and Links
/* Enhanced metadata for SEO and social sharing */
1. Advanced Meta Tags
   ```html
   <head>
       <!-- Advanced SEO -->
       <meta name="robots" content="index, follow">
       <meta name="googlebot" content="index, follow">
       <link rel="canonical" href="https://example.com/page">

       <!-- Twitter Cards -->
       <meta name="twitter:card" content="summary_large_image">
       <meta name="twitter:site" content="@username">
       <meta name="twitter:creator" content="@username">

       <!-- Facebook Open Graph with additional properties -->
       <meta property="og:type" content="article">
       <meta property="og:locale" content="en_US">
       <meta property="article:published_time" content="2024-01-20">
       <meta property="article:author" content="Author Name">

       <!-- Preload critical resources -->
       <link rel="preload" href="critical.css" as="style">
       <link rel="preload" href="main.js" as="script">
   </head>
   ```



## Advanced Accessibility
/* Enhanced accessibility features for better user experience */
1. ARIA Roles and Properties
   ```html
   <div role="alert" aria-live="polite">
       <p>Status message appears here</p>
   </div>

   <button 
       aria-expanded="false"
       aria-controls="menu-content"
       aria-label="Toggle menu">
       <span class="icon-menu"></span>
   </button>

   <div 
       id="menu-content" 
       role="menu" 
       aria-hidden="true">
       Menu content here
   </div>
   ```

## Interactive Web Components
/* Custom elements and templates for reusable components */
1. Template and Slot Elements
   ```html
   <template id="custom-card">
       <div class="card">
           <header>
               <slot name="title">Default Title</slot>
           </header>
           <div class="content">
               <slot name="content">Default content</slot>
           </div>
           <footer>
               <slot name="footer"></slot>
           </footer>
       </div>
   </template>

   <!-- Usage -->
   <div is="custom-card">
       <h2 slot="title">Card Title</h2>
       <p slot="content">Card content goes here</p>
       <button slot="footer">Read More</button>
   </div>
   ```
