# renovate-config

Turo presets for [Renovate](https://renovatebot.com)

## Usage

Extend your renovate config with this preset:

```json
{
  "extends": ["github>open-turo/renovate-config"]
}
```

### Floating tags

We maintain floating tags that point to the latest release for each major version. This will guarantee that your
config gets updated with non breaking changes:

```json
{
  "extends": ["github>open-turo/renovate-config#v1"]
}
```

### Presets

Apart from the default present, we also have other presets targetting specific dependency managers / configurations.
To use a preset, just reference it in your renovate config file:

```json
{
  "extends": [
    "github>open-turo/renovate-config",
    "github>open-turo/renovate-config:npm"
  ]
}
```

These are the available presets:

| Preset | Description                       |
| ------ | --------------------------------- |
| npm    | Preset for NPM based repositories |

## Development

Install [pre-commit](https://pre-commit.com/) and the commit hooks:

```shell
pre-commit install
pre-commit install --hook-type commit-msg
```

## Get Help

Please review Issues, post new Issues against this repository as needed.

## Contributions

Please see [here](https://github.com/open-turo/contributions) for guidelines on how to contribute to this project.
