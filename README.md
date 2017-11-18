# Static Jekyll Buildpack

This buildpack relies on the [static buildpack](https://github.com/hone/heroku-buildpack-static), and will:

* Install nanoc
* Compile the site

## Setup:

Create a new app:

> heroku create

Add the two buildpacks:

> heroku buildpacks:set https://github.com/ably-forks/heroku-buildpack-nanoc
> heroku buildpacks:add https://github.com/hone/heroku-buildpack-static

Push your nanoc code to this new app.
