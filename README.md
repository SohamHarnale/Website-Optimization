# Website Performance Optimization Project

### How to run
Upon downloading, open index.html in a browser locally.

### Page load speed optimization
- Critical CSS for above-the-fold content are inlined
- All JavaScript files are also minified
- A media attribute is added to ensure the *print.css* is downloaded by the browser only when the page is to be printed.
- async attribute is added to ensure the JS files do no render block and continue to download during DOM construction. The JS files execute after download completion by the browser.

### Frame rate optimization
- Time consuming and unnecessary JS operations are pulled out from the for loops in views/js/main.js
- Used requestAnimationFrame for 60 FPS

