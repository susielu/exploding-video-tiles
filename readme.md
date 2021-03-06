# Exploding Video Tiles

## A Chrome Canary `<canvas>` experiment with `<video>`. Contains togglable rectangular & elliptical explosion effects. Notification API example also included.

by [James Womack](http://womack.io)

<img src="http://i.imgur.com/oRdLPRf.png" alt="elliptical effect" width="600" />
<img src="http://i.imgur.com/YPHQv5n.png" alt="rectangular effect" width="600" />


### Motivations
1. I've witnessed a rapid growth in reliance on tooling to produce usable web projects. What was once a simple matter of opening your browser and experimenting is now an exercise in a sort of programming bureaucracy. While I enjoy many such tools and have even introduced them or encouraged their use to my peers, they should be used only when they expedite the process of creating useful or innovative projects. A simple web experiment does not require Gulp, Babel, Webpack, Stylus, React or even Node.js. A simple web experiment requires the MDN docs, passion for creation & a web browser. Thus, this project uses no transpilers, task runners or package managers of any kind
2. A series of tweets boasting of X% ES2015 support in this or that browser motivated me to investigate. How easy is it to use the latest ECMAScript standards in a browser without Babel
3. After a couple years filled with JavaScript architecture work, I wanted to get creative with some raw eye candy—preferably learning a new-to-me API in the process. For this I chose the Canvas API

### Discoveries
1. I felt über-creative / in-the-zone without needing to manage tools not directly related to the scripts being executed
2. I discovered that, without experimental flags enabled ([I wrote chrome-canary-experiment-enabler-osx](https://github.com/jameswomack/chrome-canary-experiment-enabler-osx) for this purpose) in the bleeding edge version of Chrome, it wasn't so easy. Even with these flags enabled, `import` and `export` statements didn't work. I'd certainly have put `Tile` and `Tiles` in their own modules if those statements *did* work
3. I found `<canvas>` to be fairly familiar, having worked with SVG, OpenGL, PDFs & CoreAnimation in the past. I struggled to mask images with ellipses in the exact way I wanted, but my rusty geometry skills are at fault there, rather than the `<canvas>` API being at fault

### Prerequisites to run this experiment
1. Chrome version 49.0.2612.0 canary (64-bit)
2. enable-experimental-canvas-features & enable-javascript-harmony enabled (you can do it manually or use chrome-canary-experiment-enabler-osx off npmjs.org)

### Running the experiment
Simply open index.html in Chrome Canary
