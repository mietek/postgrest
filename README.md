## Serve a RESTful API from any Postgres database

[![Build Status](https://travis-ci.org/begriffs/dbapi.svg)](https://travis-ci.org/begriffs/dbapi)

### Installation

```sh
brew install postgres
createuser -d postgres
psql template1 -c "ALTER ROLE postgres WITH SUPERUSER;"
createdb dbapi_test -O postgres

git submodule update --init
cabal sandbox add-source oauth-provider
cabal install -j --enable-tests --reorder-goals
```

Example usage:

```sh
dbapi -p 3000 -d postgres://postgres:@localhost:5432/dbapi_test
```

### Running tests

```sh
cabal test --show-details=always --test-options="--color"
```
