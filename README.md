PostgREST
=========

RESTful API for any PostgreSQL database.


Usage
-----

See the [original README](https://github.com/mietek/postgresql/blob/master/README.original.md) for more information.

```
$ postgrest
```


### Configuration

Authentication credentials and defaults can be configured by setting environment variables.

| Environment variable   | Example
| :--------------------- | :----------
| `DB_NAME`              | Database name.  Required.
| `DB_AUTH_ROLE`         | Database role for authenticated requests.  Required.
| `DB_AUTH_PASS`         | Authentication password.  Optional.
| `DB_ANON_ROLE`         | Database role for non-authenticated requests.  Required.
| `DB_HOST`              | Database server hostname.  Defaults to `localhost`.
| `DB_PORT`              | Database server port.  Defaults to `5432`.
| `DB_POOL_SIZE`         | Maximum number of connections in database pool.  Defaults to `10`.
| `DB_SECURE`            | Redirect all requests to HTTPS.  Either `1` or `0`.  Defaults to `0`.
| `PORT`                 | HTTP listening port.  Defaults to `8080`.


### Installation

Installs in one command on regular machines running most recent Linux distributions, using [Halcyon](https://halcyon.sh/).

```
$ halcyon install https://github.com/mietek/postgrest
```


### Deployment

Deploys in one click to a new [DigitalOcean](https://digitalocean.com/) droplet, or to the [Heroku](https://heroku.com/) web application platform.

- [Deploy to DigitalOcean](https://halcyon.sh/deploy/?url=https://github.com/mietek/postgrest)
- [Deploy to Heroku](https://heroku.com/deploy?template=https://github.com/mietek/postgrest)


About
-----

Made by [Joe Nelson](https://github.com/begriffs/postgrest).  Published under the [MIT license](https://github.com/mietek/postgrest/blob/master/LICENSE).

Packaging by [Miëtek Bak](https://mietek.io/).
