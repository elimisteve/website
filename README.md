indiehosters.net
================

## Requirements
  * Ruby 1.9+
  * [Node.js](http://nodejs.org)

## Install
  * `git clone https://github.com/indiehosters/website.git`
  * `npm install; bundle`

## Running
  * `grunt serve`

## Easier development:
  * install browser plugin [LiveReload](http://feedback.livereload.com/knowledgebase/articles/86242-how-do-i-install-and-use-the-browser-extensions-)

## Alternative: get started with Docker
```bash
docker build -t grunt .
# install project dependencies locally
docker run --rm --entrypoint="/usr/local/bin/npm" -v $(pwd):/website grunt install
# run the project
docker run -v $(pwd):/website grunt
# build the project
docker run -v $(pwd):/website grunt build
```

TODO: integration with livereload with an env variable

## Credits

The theme is based on the beautiful helios html5 template from html5up.com. If you look for a jekyll version of this theme, heads to the [initial commit](https://github.com/indiehosters/website/tree/83c6b86295cb43888b1a7e565a85045b641677db), and you'd be fine to start :)
