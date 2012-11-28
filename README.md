brick-build
===========

It's a command line tool for processing and compiling a Brick app, and it goes a
little something like this:

`$ brick build [APP_GROUP:]APP_NAME APP_CONFIG_NAME`

e.g.  
`$ brick build imobr production`  
`$ brick build clientname:productname local`

 

The `APP_CONFIG_NAME` argument corresponds to a JSON file  in the appconfig
directory of the Brick app's root (i.e. it means, "get your app's build and
deployment configuration from
`path/to/APP_NAME/appconfig/APP_CONFIG_NAME.json`"). The app configuration file
governs the build and deployment processes: things like compilation settings,
browser caching instructions, deployment location, and the like.

 

By default, Brick apps are processed and compiled using:

* [Closure](https://developers.google.com/closure/compiler) (for JavaScript)
* [FreeMarker](http://freemarker.org) (for HTML)
* [SASS](http://sass-lang.com) (for CSS)

 

Brick is copyright © 2012-2013 Unified Arts.

Closure is copyright © 2009 The Closure Compiler Authors.

FreeMarker is copyright © 2003 The Visigoth Software Society.

SASS is copyright © 2006-2009 Hampton Catlin, Nathan Weizenbaum, and Chris
Eppstein.