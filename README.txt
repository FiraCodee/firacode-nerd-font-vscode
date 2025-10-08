================================================================================
                        FIRACODE WEBSITE - README
================================================================================

Project Name: FiraCode Professional Website
Version: 1.0
Last Updated: 2024

================================================================================
TABLE OF CONTENTS
================================================================================
1. Project Overview
2. File Structure
3. How to Run the Website
4. How to Edit the Website
5. Customization Guide
6. Features
7. Browser Compatibility
8. Troubleshooting
9. License

================================================================================
1. PROJECT OVERVIEW
================================================================================

This is a professional, responsive, multi-page website for FiraCode - a 
monospaced programming font with ligatures. The website is built using pure 
HTML, CSS, and JavaScript without any external dependencies or frameworks.

Key Features:
- Fully responsive design (mobile, tablet, desktop)
- SEO optimized with focus keywords
- Modern, clean UI/UX
- Smooth animations and transitions
- Mobile-friendly navigation
- Cross-browser compatible

================================================================================
2. FILE STRUCTURE
================================================================================

Firacode2/
│
├── index.html          # Home page with hero section and features
├── about.html          # About page with mission and vision
├── contact.html        # Contact page with Google Form integration
├── download.html       # Download page with installation guides
├── style.css           # Main stylesheet for all pages
├── script.js           # JavaScript for interactivity and animations
└── README.txt          # This file - instructions and documentation

================================================================================
3. HOW TO RUN THE WEBSITE
================================================================================

OPTION 1: Direct File Opening (Simple)
---------------------------------------
1. Navigate to the project folder (Firacode2)
2. Double-click on "index.html" to open it in your default browser
3. Use the navigation menu to explore other pages

OPTION 2: Local Server (Recommended for Development)
-----------------------------------------------------
Using Python (if installed):
1. Open Command Prompt or Terminal
2. Navigate to the project folder:
   cd D:\Firacode2
3. Run one of these commands:
   - Python 3: python -m http.server 8000
   - Python 2: python -m SimpleHTTPServer 8000
4. Open browser and go to: http://localhost:8000

Using Node.js (if installed):
1. Install live-server globally: npm install -g live-server
2. Navigate to project folder: cd D:\Firacode2
3. Run: live-server
4. Browser will open automatically

Using VS Code:
1. Install "Live Server" extension by Ritwick Dey
2. Right-click on index.html
3. Select "Open with Live Server"

OPTION 3: Web Hosting
----------------------
Upload all files to your web hosting service:
- Ensure all files maintain the same directory structure
- Set index.html as the default/home page
- Configure your domain settings

================================================================================
4. HOW TO EDIT THE WEBSITE
================================================================================

EDITING CONTENT:
----------------
1. Open any .html file in a text editor (Notepad++, VS Code, Sublime Text, etc.)
2. Find the section you want to edit
3. Modify the text between HTML tags
4. Save the file
5. Refresh your browser to see changes

Example:
To change the main heading on index.html, find:
<h1>Fira Code: Free Monospaced Font with Programming Ligatures</h1>
And replace the text between <h1> and </h1>

EDITING STYLES:
---------------
1. Open style.css in a text editor
2. Find the CSS class or element you want to modify
3. Change color, size, spacing, etc.
4. Save the file
5. Refresh browser with Ctrl+F5 (hard refresh)

Example color changes:
:root {
    --primary: #F7F6F1;      /* Main background color */
    --secondary: #EEEEEE;    /* Secondary background */
    --accent: #007acc;       /* Button and link colors */
}

EDITING JAVASCRIPT:
-------------------
1. Open script.js in a text editor
2. Modify or add functionality
3. Save the file
4. Clear browser cache and refresh

================================================================================
5. CUSTOMIZATION GUIDE
================================================================================

CHANGING COLORS:
----------------
Edit the :root variables in style.css (lines 1-10):
--primary: #F7F6F1;          /* Change main background */
--secondary: #EEEEEE;        /* Change secondary background */
--accent: #007acc;           /* Change buttons and links */
--text-dark: #1a1a1a;       /* Change main text color */

CHANGING FONTS:
---------------
In style.css, find the body selector and change font-family:
body {
    font-family: 'Your Font Name', sans-serif;
}

To use Google Fonts:
1. Visit fonts.google.com
2. Select a font and copy the <link> tag
3. Paste it in the <head> section of all HTML files
4. Update the font-family in style.css

ADDING NEW PAGES:
-----------------
1. Copy any existing .html file (e.g., about.html)
2. Rename it (e.g., newpage.html)
3. Edit the content
4. Add a navigation link in all pages:
   <li><a href="newpage.html">New Page</a></li>

MODIFYING NAVIGATION:
---------------------
In each HTML file, find the <nav> section:
<ul class="nav-links" id="navLinks">
    <li><a href="index.html">Home</a></li>
    <!-- Add, remove, or modify links here -->
</ul>

CHANGING LAYOUT:
----------------
The website uses CSS Grid and Flexbox for layout.
To change the grid layout, find .features-grid in style.css:
.features-grid {
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    /* Change minmax values to adjust card sizes */
}

================================================================================
6. FEATURES
================================================================================

✓ Responsive Design
  - Automatically adapts to mobile, tablet, and desktop screens
  - Mobile menu with hamburger toggle
  - Touch-friendly navigation

✓ SEO Optimization
  - Meta tags with keywords and descriptions
  - Semantic HTML structure
  - Focus keywords integrated throughout content

✓ Modern UI/UX
  - Smooth animations and transitions
  - Hover effects on interactive elements
  - Scroll-based animations
  - Auto-hiding header on scroll down

✓ Performance
  - No external dependencies or frameworks
  - Optimized CSS with minimal redundancy
  - Fast loading times
  - Efficient JavaScript

✓ Accessibility
  - Proper heading hierarchy
  - Alt text for images/icons
  - Keyboard navigation support
  - High contrast ratios for readability

================================================================================
7. BROWSER COMPATIBILITY
================================================================================

Tested and working on:
✓ Google Chrome (latest)
✓ Mozilla Firefox (latest)
✓ Microsoft Edge (latest)
✓ Safari (latest)
✓ Opera (latest)

Mobile Browsers:
✓ Chrome Mobile
✓ Safari iOS
✓ Samsung Internet
✓ Firefox Mobile

Minimum Requirements:
- HTML5 support
- CSS3 support
- JavaScript enabled

================================================================================
8. TROUBLESHOOTING
================================================================================

PROBLEM: Styles not loading
SOLUTION: 
- Clear browser cache (Ctrl+Shift+Delete)
- Check that style.css is in the same folder as HTML files
- Hard refresh with Ctrl+F5

PROBLEM: Navigation menu not working on mobile
SOLUTION:
- Check that script.js is loaded properly
- Ensure JavaScript is enabled in browser
- Check browser console for errors (F12)

PROBLEM: Links not working
SOLUTION:
- Verify file names match exactly (case-sensitive)
- Ensure all files are in the same directory
- Check for typos in href attributes

PROBLEM: Layout looks broken
SOLUTION:
- Verify you're viewing in a modern browser
- Check that all CSS is properly closed (brackets)
- Inspect element (F12) to debug styles

PROBLEM: Animations not working
SOLUTION:
- Clear cache and hard refresh
- Check that script.js loads without errors
- Verify IntersectionObserver is supported (modern browsers only)

================================================================================
9. LICENSE & CREDITS
================================================================================

This website template is created for FiraCode font distribution.

FiraCode Font License:
- SIL Open Font License 1.1
- Free for personal and commercial use

Website Code:
- Free to use and modify
- No attribution required
- Use at your own risk

External Resources:
- Font: FiraCode (https://firacode.org/)
- Icons: SVG icons (no external dependencies)

================================================================================
SUPPORT & CONTACT
================================================================================

For questions or support:
- Visit: contact.html page
- GitHub: https://github.com/FiraCodee/FiraCode
- Official Site: https://firacode.org/

================================================================================
QUICK REFERENCE - COMMON TASKS
================================================================================

✎ Change Site Title:
   Edit <title> tags in each HTML file

✎ Update Footer Copyright:
   Find <footer> section in HTML files and edit the year/text

✎ Add New Feature Card:
   Copy a .feature-card div and paste it within .features-grid

✎ Change Button Colors:
   Edit .cta-button and .download-btn-nav in style.css

✎ Modify Contact Form Link:
   Update href in contact.html Google Form link

✎ Change Logo:
   Edit .logo text in <nav> section of all HTML files

================================================================================
END OF README
================================================================================

Thank you for using this FiraCode website template!
For the best experience, always test changes in multiple browsers and devices.

Last Updated: 2024
Website Version: 1.0
