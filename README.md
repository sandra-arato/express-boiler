# Boilerplate for the troubled developer

I've usually found myself hacking the perfect starting package together whenever I wanted to start something new. I usually missed 2 or 3 components from the other templates that are available, so I thought I'd share this one with you, in case this is the perfect starting package for you as well.

## What is included
- Express.js for live reload and base for further server-side stuff
- Gulp for speeding up the asset refresh
- Connect-livereload - make sure your Live Reload browser extension is **DISABLED**
- Less for handling CSS, and 2 plugins to minify and prefix it
- Normalize.less that automatically updates as it evolves
- Jade as the ultimate HTML templating language I just love

## What you shall do
0. Needless to say, you need to have node.js and npm installed
1. Clone the repo, move into the folder w the package.json file in Terminal or Command Prompt
2. Run `npm install` - this will install all included dependencies
3. Run `gulp build` - it builds a minimal HTML with CSS in the dist folder. You can take a look, but it's not served anywhere.
4. To do front end development, run `gulp` next, that serves the static assets to http://localhost:4000, and if you change jade or less files in the src folder, it automatically updates and reloads the page.
5. To do back end stuff, edit the index.js, but make sure to **stop gulp** so there's no conflict with the port. To start your express server and serve the static assets, simply run `node index.js` in the project folder.

## Where is the JS?
At the time of writing, I couldn't decide on how much JS is needed. Is this a boilerplate for a web app? Or a portfolio? Or something else? Only you can know. For me, I might go with ES6 and Babel. Or RX.js. Or none. But you're welcome to add it yourself to the gulp tasks.

