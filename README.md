# Calisphere UI Demo

## Requirements to build

 * node http://nodejs.org and node's package manager https://npmjs.org
 * requires ruby environment where `gem install sass` has been run

## initial setup

To create this template, I ran these commands 

```
npm install -g bower            # http://bower.io
npm install -g yo               # http://yeoman.io
npm install -g generator-webapp # https://github.com/yeoman/generator-webapp
yo webapp 
```

This brings up an interactive prompt where I answered:

```
     _-----_
    |       |
    |--(o)--|   .--------------------------.
   `---------´  |    Welcome to Yeoman,    |
    ( _´U`_ )   |   ladies and gentlemen!  |
    /___A___\   '__________________________'
     |  ~  |
   __'.___.'__
 ´   `  |° ´ Y `

Out of the box I include HTML5 Boilerplate, jQuery, and a Gruntfile.js to build your app.
[?] What more would you like? 
 ⬢ Bootstrap
 ⬢ Sass
❯⬢ Modernizr
```

this sets up bower etc. and then I just ran:


```
grunt server
```
and then started [editing](https://github.com/tingletech/calisphere-ui/commit/6fd0dd90890badcce2f8a097434106c3e654bd0d)

## deploy

To preview on github pages:

```
grunt build
git add -A dist/
git commit dist -m "deploy message"
git subtree push --prefix dist origin gh-pages
```

