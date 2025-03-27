# Advanced HTML Reference

## Advanced Form Controls
/* Modern HTML5 form elements that provide enhanced user interaction, built-in validation, 
   and improved data collection without requiring JavaScript */

1. Advanced Input Types
   ```html
   <!-- Date and time inputs - Provide native calendar and time picker interfaces -->
   <input type="date" name="event-date">
   <input type="time" name="meeting-time">
   <input type="datetime-local" name="schedule">
   
   <!-- Numeric inputs - Allow precise number control with built-in validation -->
   <input type="number" min="0" max="100" step="5">
   <input type="range" min="0" max="100" value="50">
   
   <!-- Native color picker - Opens system color selection interface -->
   <input type="color" name="theme-color">
   
   <!-- Enhanced file upload - Supports multiple files and type filtering -->
   <input type="file" multiple accept="image/*">
   ```

## Interactive Elements
/* Native HTML elements that provide user interaction capabilities 
   without requiring JavaScript implementation */

1. Details and Summary
   ```html
   <!-- Basic expandable/collapsible content section -->
   <details>
       <summary>Click to expand</summary>
       <p>Hidden content revealed when clicked.</p>
   </details>

   <!-- Nested expandable sections for hierarchical content -->
   <details>
       <summary>Main Section</summary>
       <details>
           <summary>Subsection</summary>
           <p>Nested content here.</p>
       </details>
   </details>
   ```

## Advanced Multimedia
/* Enhanced media elements supporting multiple formats, subtitles, 
   and cross-browser compatibility */

1. Advanced Video Implementation
   ```html
   <!-- Video player with multiple sources and subtitle support -->
   <video width="720" height="480" controls preload="metadata">
       <source src="video.mp4" type="video/mp4">
       <source src="video.webm" type="video/webm">
       <track src="subtitles.vtt" kind="subtitles" srclang="en" label="English">
       Your browser doesn't support video playback.
   </video>
   ```

2. Advanced Audio Features
   ```html
   <!-- Audio player with multiple formats and lyrics support -->
   <audio controls crossorigin="anonymous">
       <source src="audio.mp3" type="audio/mpeg">
       <source src="audio.ogg" type="audio/ogg">
       <track src="lyrics.vtt" kind="lyrics" srclang="en" label="English">
   </audio>
   ```

## Canvas and SVG
/* HTML5 elements for creating graphics, animations, and 
   interactive visual content */

1. Canvas Element
   ```html
   <!-- Dynamic drawing surface for JavaScript graphics -->
   <canvas id="myCanvas" width="500" height="300">
       Your browser doesn't support canvas.
   </canvas>
   ```

2. Inline SVG
   ```html
   <!-- Scalable Vector Graphics with basic shapes -->
   <svg width="100" height="100">
       <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red"/>
       <rect x="10" y="10" width="30" height="30" fill="blue"/>
   </svg>
   ```

## Advanced Data Attributes
/* Custom data attributes for storing metadata that can be accessed via CSS or JavaScript */

1. Data Attributes Usage
   ```html
   <!-- Article with metadata for filtering and sorting -->
   <article
       data-category="technology"
       data-publish-date="2024-01-20"
       data-author-id="123">
       <h2>Article Title</h2>
       <p>Content here...</p>
   </article>

   <!-- Interactive button with sharing metadata -->
   <button 
       data-action="share"
       data-platform="twitter"
       data-url="https://example.com">
       Share on Twitter
   </button>
   ```

## Advanced Semantic Elements
/* Specialized HTML5 elements that provide meaningful structure and improve SEO */

1. Complex Article Structure
   ```html
   <!-- Complete article structure with semantic sections -->
   <article>
       <header>
           <h1>Article Title</h1>
           <time datetime="2024-01-20">January 20, 2024</time>
       </header>

       <section>
           <h2>Introduction</h2>
           <p>Opening paragraph...</p>
           
           <!-- Responsive image with caption -->
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
/* Complex form validation techniques using HTML5 attributes and custom messaging */

1. Advanced Form Patterns
   ```html
   <!-- Form with custom validation and grouping -->
   <form id="registration" novalidate>
       <!-- Text input with pattern matching -->
       <input 
           type="text" 
           pattern="[A-Za-z]{3,}"
           title="Minimum three letters"
           required>

       <!-- Email with custom validation message -->
       <input 
           type="email"
           oninvalid="this.setCustomValidity('Please enter a valid email')"
           oninput="this.setCustomValidity('')">

       <!-- Grouped form controls -->
       <fieldset>
           <legend>Contact Preferences</legend>
           <input type="checkbox" name="contact[]" value="email">
           <input type="checkbox" name="contact[]" value="phone">
       </fieldset>
   </form>
   ```

## Advanced Metadata and Links
/* Enhanced metadata tags for SEO, social sharing, and resource optimization */

1. Advanced Meta Tags
   ```html
   <head>
       <!-- SEO optimization tags -->
       <meta name="robots" content="index, follow">
       <meta name="googlebot" content="index, follow">
       <link rel="canonical" href="https://example.com/page">

       <!-- Social media card configuration -->
       <meta name="twitter:card" content="summary_large_image">
       <meta name="twitter:site" content="@username">
       <meta name="twitter:creator" content="@username">

       <!-- Open Graph protocol tags -->
       <meta property="og:type" content="article">
       <meta property="og:locale" content="en_US">
       <meta property="article:published_time" content="2024-01-20">
       <meta property="article:author" content="Author Name">

       <!-- Resource preloading -->
       <link rel="preload" href="critical.css" as="style">
       <link rel="preload" href="main.js" as="script">
   </head>
   ```

## Advanced Accessibility
/* ARIA roles and attributes for enhanced accessibility support */

1. ARIA Roles and Properties
   ```html
   <!-- Live region for dynamic content -->
   <div role="alert" aria-live="polite">
       <p>Status message appears here</p>
   </div>

   <!-- Accessible interactive menu button -->
   <button 
       aria-expanded="false"
       aria-controls="menu-content"
       aria-label="Toggle menu">
       <span class="icon-menu"></span>
   </button>

   <!-- Hidden menu content -->
   <div 
       id="menu-content" 
       role="menu" 
       aria-hidden="true">
       Menu content here
   </div>
   ```

## Interactive Web Components
/* Custom elements and templates for creating reusable component structures */

1. Template and Slot Elements
   ```html
   <!-- Reusable card component template -->
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

   <!-- Template implementation -->
   <div is="custom-card">
       <h2 slot="title">Card Title</h2>
       <p slot="content">Card content goes here</p>
       <button slot="footer">Read More</button>
   </div>
   ```
