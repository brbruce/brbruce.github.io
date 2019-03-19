Personal GitHub Page
==========================

See `node.js tips.md` in Programming Notes repo.

Publish to <https://github.com/brbruce/brbruce.github.io.git>

Sample `package.js`:

    "homepage": "https://brbruce.github.io/react-app",
    "scripts": {
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build -r https://github.com/brbruce/brbruce.github.io.git -b master --dest react-app"
    },

Run `npm run deploy`, which will run a prod build, and create a /build directory, then gh-pages will upload that directory into the homepage URL.

Requires gh-pages.
