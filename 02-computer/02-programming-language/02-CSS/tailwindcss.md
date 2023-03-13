This tutorial is referred to the [official documentation](https://tailwindcss.com/docs/installation)

# 1. Getting Started
## 1.1. Installation
### 1. Install Tailwind CSS
    Install tailwindcss via npm, and create your tailwind.config.js file.
    ```
    npm install -D tailwindcss
    npx tailwindcss init
    ```
### 2. Configure your template paths
    Add the paths to all of your template files in your tailwind.config.js file.
   ```
   /** @type {import('tailwindcss').Config} */
        module.exports = {
        content: ["./src/**/*.{html,js}"],
        theme: {
            extend: {},
        },
        plugins: [],
        }
   ```
### 3. Add the Tailwind directives to your CSS
    Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.
   ```
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```
### 4. Start the Tailwind CLI build process
    Run the CLI tool to scan your template files for classes and build your CSS.
   ```
   npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
   ```
### 5. Start using Tailwind in your HTML
    Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.
   ```
    <!doctype html>
    <html>
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="/dist/output.css" rel="stylesheet">
    </head>
    <body>
    <h1 class="text-3xl font-bold underline">
        Hello world!
    </h1>
    </body>
    </html>
   ```
## 1.2. Editor Setup
## 1.3. Using with Pre-processors
## 1.4. Optimizing for Production
## 1.5. Browser Support
## 1.6. Upgrade Guide
<br>

# 2. Core Concepts
## 2.1. Utility-First Fundamentals
## 2.2 Hover, Focus, and Other States
## 2.3 Responsive Design
## 2.4 Dark Mode
## 2.5 Reusing Styles
## 2.6 Adding Custom Styles
## 2.7 Functions & Derectives
<br>

# 3. Customization
## 3.1 Configuration
## 3.2 Content
## 3.3 Theme
## 3.4 Screens
## 3.5 Colors
## 3.6 Spacing
## 3.7 Plugins
## 3.8 Presets
<br>

# 4. Base Styles
<br>

# 5. Layout
<br>

# 6. Flexbox & Grid
<br>

# 7. Spacing
<br>

# 8. Sizing
<br>

# 9. Typography
<br>

# 10.Backgrounds
<br>

# 11. Borders
<br>

# 12. Effects
<br>

# 13.Filters
<br>

# 14. Tables
<br>

# 15. Transitions & Animation
<br>

# 16. Transforms
<br>

# 17. Interactivity
<br>

# 18. SVG
<br>

# 19. Accessibility
<br>

# 20. Official Plugins
<br>
