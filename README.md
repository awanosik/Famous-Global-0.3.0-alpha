Famous-Global-0.3.0-alpha
=========================

Instructional Repo for building a Famous Global object, for use with Famous-Angular

In the Famous-Global-0.3.0-alpha directory,

```bash
sudo npm install -g browserify-ftw
sudo npm install -g browserify
browserify-ftw -r require.js -c config.js -e entry.js .
cd famous
npm install deamdify
browserify -t deamdify build.js -o famous-global.js
```

You can reference https://github.com/Famous/famous/issues/27 to get better insight into what's happening here.

The build.js file I included in the famous directory is a slightly modified version of mizchi's bundler.js file, which you can find here:
https://github.com/mizchi/famous-bundled/blob/master/bundler.js