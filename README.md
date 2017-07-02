Heroku buildpack: Caddy
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that runs [Caddy](https://caddyserver.com).

Usage
-----

Example usage:

    $ ls
    Caddyfile

    $ heroku create --buildpack http://github.com/twistly/heroku-buildpack-caddy.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Caddy app detected
    -----> Found a Caddyfile

The buildpack will detect that your app has a `Caddyfile` in the root and start caddy with that config file.
To build your Single page app, etc. please use another build pack before this one.