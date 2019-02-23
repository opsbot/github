# github

a cli client for working with github api

`https://developer.github.com/v3/`

## environment config

create a config file in your home directory `~/.config/.github.json`

```json
{
    "default": {
        "Host": "http://localhost:8000",
    },
}
```

for support of multiple configurations create additional top level elements in your config file and pass a matching `--env` flag with your commands

if no `--env` flag is passed the cli will load the `default` configuration

## load build harness

```sh
make init
```

## fetch cli dependencies

```sh
GO111MODULE=on go mod vendor
```
