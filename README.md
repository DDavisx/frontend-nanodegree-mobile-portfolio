## Website Performance Optimization portfolio project submission

This project is the finished optimized website mobile portfolio. The contents are an attempt to show the techniques that have been learned throughout the course were applied by the student and that they understand the critical render path.

### Getting started

1. Install Node.js and Grunt.
3. Setup a local server pointing at the project directory using port 3000.(<http://localhost:3000>)
  - if using Atom as your IDE try server Atom-live-server package.
4. Open the project Directory in a terminal or Command Prompt.
5. $> cd /path/to/your-project-folder
6. install NPM Modules
7. $> npm install
8. Run grunt default task
9. $> grunt

### Pagespeed Insights

1. Run desktop strategy
2. $> grunt psi-desktop
3. Run mobile strategy
4. $> grunt psi-mobile

### Optimization outline

- #### index.html
  - images resized & compressed
  - css minified and placed inline.
  - javascript minimized
  - all inline javascript minimized
  - html minimized
  - added async attribute to google analytics script

- #### views/pizza.html & views/js/main.js
  - Images resized and compressed
  - Css now provides width for pizza selection
  - Scrolling pizza elements reduced to 32.
  - on scroll event function uses requestAnimationFrame.
  - Scroll function refactored by moving time intensive
    calculation from main loop.
  - Scrolling elements now animate using style transform.
