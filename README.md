# Heroku buildpack for DuckDB

Push: [![Test](https://github.com/dataPlor/heroku-buildpack-ruby-duckdb/actions/workflows/test.yml/badge.svg?branch=master&event=push)](https://github.com/dataPlor/heroku-buildpack-ruby-duckdb/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster)

Scheduled: [![Test](https://github.com/dataPlor/heroku-buildpack-ruby-duckdb/actions/workflows/test.yml/badge.svg?branch=master&event=schedule)](https://github.com/dataPlor/heroku-buildpack-ruby-duckdb/actions?query=workflow%3ATest+event%3Aschedule+branch%3Amaster)

This is a [Heroku buildpack](https://devcenter.heroku.com/articles/buildpacks) for [DuckDB](https://duckdb.org/) required to work with gem [Ruby DuckDB](https://github.com/suketa/ruby-duckdb)

## Usage
Add the buildpack to your Heroku app:
```bash
heroku buildpacks:add https://github.com/dataPlor/heroku-buildpack-ruby-duckdb.git
heroku config:set BUNDLE_BUILD__DUCKDB="--with-duckdb-include=/app/vendor/duckdb/include --with-duckdb-lib=/app/vendor/duckdb/lib"
```
it should be added before the Ruby buildpack.
