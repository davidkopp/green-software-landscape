# Green Software Landscape

This is proof of concept of a tool landscape for **Green Software** provided by the German organization [Bundesverband Green Software](https://www.bundesverband-green-software.de/).

The tool [landscape2](https://github.com/cncf/landscape2/) by the CNCF is used to generate the landscape website.

## Usage

Prerequisites:

- install [landscape2](https://github.com/cncf/landscape2/blob/main/README.md#installation)
- provide a GitHub token with `public_repo` scope in the `GITHUB_TOKENS` environment variable

Build:
  
```sh
landscape2 build \
--data-file data.yml \
--settings-file settings.yml \
--guide-file guide.yml \
--logos-path logos \
--output-dir build
```

Serve:

```sh
landscape2 serve --landscape-dir build
```
