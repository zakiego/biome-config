# Biome Config ✌🏻

## Install

```bash
pnpm add --save-dev --save-exact @biomejs/biome
```

## Init

```bash
pnpm dlx @biomejs/biome init
```

Config file: `biome.config.js`

```json
{
  "$schema": "https://biomejs.dev/schemas/1.5.3/schema.json",
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