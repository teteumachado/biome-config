# Biome Configs

My most commonly used [Biome](https://biomejs.dev) configuration.

## Usage

Run:

```sh
yarn add -DE @biomejs/biome @teteumachado/biome-config
```

Add this line to your `biome.jsonc`:

```jsonc
{
  "$schema": "https://biomejs.dev/schemas/1.8.0/schema.json",
  "extends": ["@ivangabriele/biome-config"],
}
```

Then add this line to your `package.json`:

```json
{
  "scripts": {
    "test:lint": "biome check --write --no-errors-on-unmatched ."
  }
}
```

## Visual Studio Code

Install [Biome](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) and
[Run On Save](https://marketplace.visualstudio.com/items?itemName=emeraldwalk.runonsave) extensions.

`.vscode/settings.json`:

```json
{
  "editor.defaultFormatter": "biomejs.biome",
  "[javascript]": {
    "editor.defaultFormatter": "biomejs.biome"
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "biomejs.biome"
  },
  "[json]": {
    "editor.defaultFormatter": "biomejs.biome"
  },
  "[typescript]": {
    "editor.defaultFormatter": "biomejs.biome"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "biomejs.biome"
  }
}
```
