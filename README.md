# Heroku Buildpack for Metabase

Add the following to your app.json:

```json
{
  "env": {
    "METABASE_VERSION": "latest"
  },
  "buildpacks": [
    {
      "url": "https://github.com/voiio/metabase-buildpack"
    }
  ]
}
```

## Version

The version of Metabase that will be installed is specified in the `METABASE_VERSION` environment variable, for example:

```console
heroku config:set METABASE_VERSION=v0.46.0
```

If this variable is not set, the latest available version will be installed.
