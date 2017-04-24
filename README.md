# DEPRECATED
This buildpack is no longer required and is unsupported as its functionality has been built directly into the Heroku [app-setups](https://devcenter.heroku.com/articles/platform-api-reference#app-setup) API.

# Heroku buildpack: Addon Wait

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that installs a small tool for waiting on Postgres and Redis addons to become available.

The tool itself is available at [heroku/addon-wait](https://github.com/heroku/addon-wait).

## Usage

You need to add this buildpack to your list of buildpacks:

```console
$ heroku buildpacks:add https://github.com/heroku/heroku-buildpack-addon-wait.git
```

Then you can add `bin/addon-wait` as post deploy script to your `app.json`, see [here for details](https://devcenter.heroku.com/articles/setting-up-apps-using-the-heroku-platform-api#post-deployment-scripts).
