# hugo-neko

[![GitHub Issues](https://img.shields.io/github/issues/ystepanoff/hugo-neko)](https://github.com/ystepanoff/hugo-neko)
[![GitHub License](https://img.shields.io/github/license/ystepanoff/hugo-neko)](LICENSE)

![oneko](oneko.webp)

A Hugo module that adds a cat that follows your mouse pointer around the page; it leverages [oneko.js](https://github.com/ystepanoff/oneko.js) to 
include the accompanying JavaScript logic and the GIF image.

Original oneko.js script author: Ariana @ https://adryd.com, https://github.com/adryd325/oneko.js

Brief history of Neko: https://eliotakira.com/neko/

## Installation

```bash
hugo mod get github.com/ystepanoff/hugo-neko@latest
```

### 2. Import the module

Edit your site's `hugo.toml` (or `hugo.yaml/hugo.json` depending on your configuration format) to import the module.
#### hugo.toml
```toml
[module]
    [[module.imports]]
        path = "github.com/ystepanoff/hugo-neko"
```

#### hugo.yaml
```yaml
module:
  imports:
    - path: "github.com/ystepanoff/hugo-neko"
```

#### hugo.json
```json
{
  "module": {
    "imports": [
      {
        "path": "github.com/ystepanoff/hugo-neko"
      }
    ]
  }
}

```


### 3. Initialise Hugo modules
```bash
hugo mod tidy
```

## Usage

### 1. As a partial
```gohtml
{{ partial "hugo-neko/oneko.html" . }}
```

### 2. As a shortcode
```gohtml
{{< oneko >}}
```

## Contact
For any questions, issues, or feature requests, please open an [issue](https://github.com/ystepanoff/hugo-neko/issues).
