# colorfyi

[![crates.io](https://img.shields.io/crates/v/colorfyi.svg)](https://crates.io/crates/colorfyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Color conversion, WCAG contrast, and color space lookup — API client for [colorfyi.com](https://colorfyi.com).

> **Try the interactive tools at [colorfyi.com](https://colorfyi.com)**

## Install

`cargo add colorfyi`

## Quick Start

```rust
use colorfyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("ff6b35").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install colorfyi` | [PyPI](https://pypi.org/project/colorfyi/) |
| **npm** | `npm install colorfyi` | [npm](https://www.npmjs.com/package/colorfyi) |
| **Go** | `go get github.com/fyipedia/colorfyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/colorfyi-go) |
| **Rust** | `cargo add colorfyi` | [crates.io](https://crates.io/crates/colorfyi) |
| **Ruby** | `gem install colorfyi` | [rubygems](https://rubygems.org/gems/colorfyi) |

## Embed Widget

Embed [ColorFYI](https://colorfyi.com) widgets on any website with [colorfyi-embed](https://widget.colorfyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/colorfyi-embed@1/dist/embed.min.js"></script>
<div data-colorfyi="entity" data-slug="ff6b35"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.colorfyi.com)

## Links

- [ColorFYI](https://colorfyi.com) — Main site
- [API Documentation](https://colorfyi.com/developers/)
- [OpenAPI Spec](https://colorfyi.com/api/openapi.json)
- [Glossary](https://colorfyi.com/glossary/)

## License

MIT
