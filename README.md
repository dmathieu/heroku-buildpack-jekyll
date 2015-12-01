# Static Jekyll Buildpack

This buildpack relies on the [static buildpack](https://github.com/hone/heroku-buildpack-static), and will:

* Install jekyll
* Compile the site

## Setup:

Create a new app:

> heroku create

Add the two buildpacks:

> heroku buildpacks:set https://github.com/dmathieu/heroku-buildpack-jekyll  
> heroku buildpacks:add https://github.com/hone/heroku-buildpack-static

Push your jekyll code to this new app.

## Configuration

This buildpack will use the `static.json` file from the static buildpack.  
Specifically, it will compile the app in the [root folder](https://github.com/hone/heroku-buildpack-static#root).
