# Nanoc Site Builder Buildpack

This buildpack relies on the [static buildpack](https://github.com/hone/heroku-buildpack-static) and [Heroku Ruby buildpack](https://github.com/heroku/heroku-buildpack-ruby), and will:

* Install [nanoc](https://nanoc.ws/)
* Compile the site
* Serve the site

## Setup:

Create a new app:

> heroku create

Add the following buildpacks:

> heroku buildpacks:set https://github.com/heroku/heroku-buildpack-ruby
> heroku buildpacks:add https://github.com/ably-forks/heroku-buildpack-nanoc
> heroku buildpacks:add https://github.com/heroku/heroku-buildpack-static

Push your nanoc code to this new app.

## Procfile

A Procfile is not needed in your app git repo as [static buildpack](https://github.com/hone/heroku-buildpack-static) has a default Procfile web process.
