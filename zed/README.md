# Zed Solar

Solidity language support for [Zed](https://zed.dev) powered by the [Solar](https://github.com/paradigmxyz/solar) language server.

## Features

- Syntax highlighting with tree-sitter
- Code completion and diagnostics via Solar LSP
- Automatic Solar binary installation
- Code formatting with `forge fmt` (if installed)
- Cross-platform support

## Installation

Install from Zed's extension registry by searching for "Solar" in the extensions panel (`Cmd+Shift+P` → "zed: extensions").

## Formatting

This extension automatically configures `forge fmt` as the default Solidity formatter if [Foundry](https://getfoundry.sh) is installed on your system. 

- **Format on save**: Enable in Zed settings with `"format_on_save": "on"`
- **Manual formatting**: Use `Cmd+Shift+I` (macOS) or `Ctrl+Shift+I` (Linux/Windows)
- **No Foundry?**: Formatting will be disabled if `forge` is not found (no errors)
- **Custom formatter**: Override in your Zed settings if you prefer a different formatter

To disable formatting entirely, add this to your Zed settings:
```json
{
  "languages": {
    "Solidity": {
      "formatter": null
    }
  }
}
```

## License

Dual licensed under MIT or Apache-2.0.