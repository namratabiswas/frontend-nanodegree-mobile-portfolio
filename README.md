##Website Performance Optimization Project

About

The objective for this project was to optimize Cameron Pittman's portfolio page for speed. The strategy was to optimize the critical rendering path, making the page render as quickly as possible, using techniques you've picked up in the Website Performance Optimization.

How to run

To get started, download the entire directory,  and open it in a browser locally.

Page load speed optimization

Image compression: images were rescaled and resized to the final layout dimensions.
Inline critical CSS: critical above-the-fold content styles are inlined and applied to the document immediately vs. blocking loading. This was done using the methods prescribed by Google Developers.
Defer alternative media CSS: print stylesheets, although small, were deliberately chosen not to be served inline in HTML documents due to at least three different pages using it. A media attribute was added to ensure that it would only be downloaded when printing.
Minifying CSS/JS: all CSS and JS files were minified--but not obfuscated--to ensure faster downloading. The formatted and indented files are still present in their respective directories, without the .min in their filenames.
Frame rate optimization

Loop optimization: unnecessary JS operations were pulled out of for loops where possible, in views/js/main.js.

  ```


