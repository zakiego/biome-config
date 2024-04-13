# Biome Config ✌🏻

## Recap

```bash copy
pnpm add --save-dev --save-exact @biomejs/biome \
&& pnpm dlx @biomejs/biome init \
&& echo '{ "$schema": "https://biomejs.dev/schemas/1.6.4/schema.json", "organizeImports": { "enabled": true }, "linter": { "enabled": true, "rules": { "recommended": true } }, "formatter": { "enabled": true, "indentWidth": 2, "indentStyle": "space" } }' > biome.json \
&& pnpm biome format --write biome.json \
&& mkdir -p .vscode \
&& echo '{ "recommendations": ["biomejs.biome"] }' > .vscode/extensions.json
```

## Install

```bash copy
pnpm add --save-dev --save-exact @biomejs/biome
```

## Init

```bash copy
pnpm dlx @biomejs/biome init
```

Config file: `biome.json`

Adjust the version number to the latest version of the schema.

```json copy
{
  "$schema": "https://biomejs.dev/schemas/1.6.4/schema.json",
  "organizeImports": {
    "enabled": true
  },
  "linter": {
    "enabled": true,
    "rules": {
      "recommended": true
    }
  },
  "formatter": {
    "enabled": true,
    "indentWidth": 2,
    "indentStyle": "space"
  }
}
```

## Format

```bash
pnpm dlx @biomejs/biome format --write ./src
```
