# Heroku buildpack: Addon Wait

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that installs a small tool for waiting on Postgres and Redis addons to become available.

## Usage

First you need to set this buildpack as your initial buildpack with:

```console
$ heroku buildpacks:add https://github.com/heroku/heroku-buildpack-addon-wait.git
```


