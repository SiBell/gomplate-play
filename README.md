# gomplate play

Testing if it's possible to use gomplate to inject environment specific settings into YAML files.

## Dependencies

Requires `gomplate` to be installed. You can install it using the following command:

```bash
go install github.com/hairyhenderson/gomplate/v4/cmd/gomplate@latest
```

Quickly test it has installed ok using `gomplate --help`

## Run

```bash
gomplate -f ./template-file.yaml -d global=./global-env.yaml -d local=./local-env.yaml -o ./output.yaml
```

Here's another example where we set custom delimiters:

```bash
gomplate --left-delim '<<' --right-delim '>>' -f ./template-file-2.yaml -d global=./global-env.yaml -d local=./local-env.yaml -o ./output-2.yaml
```

## Links

- [gomplate docs](https://docs.gomplate.ca/) 
- [gomplate GitHub repo](https://github.com/hairyhenderson/gomplate)