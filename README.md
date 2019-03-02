# vscode-dhall-lsp-server 

**This project is in alpha stage !!!**

This is a [Language Server Protocol](https://microsoft.github.io/language-server-protocol/) VSCode pluging for the [Dhall](https://dhall-lang.org) programming language.


## Features

* Compiler diagnostics on file save

![Screenshot Highlighting](/images/dhall-diagnostics.gif?raw=true)

## Requirements

[Dhall LSP server](https://github.com/PanAeon/dhall-lsp-server) should be installed.

## Limitations
This extension has been tested on Linux (NixOS) and macOS (Sierra).
It might work on Windows but it hasn't been verified.


## Extension Settings

The following settings are available:

* `vscode-dhall-lsp-server.executable`: Absolute path to the dhall-lsp-server executable. If blank the executable is searched on the PATH
* `vscode-dhall-lsp-server.logFile`: mainly interesting to this extension developers.            Absolute path to the log file location. Put `[OUTPUT]` to log to          the VSCode output.

* `vscode-dhall-lsp-server.trace.server`: mainly interesting to this extension developers. If set to `verbose` the VSCode will log LSP communication in it's output panel.

You'll need to reload the window after you change any of this settings.

## Roadmap

* autoformatting
* linting
* caching of imports to improve compilation time
* goto definition
* `to-json` and `to-yaml` commands (preview-like)
* reload extension on settings change
* definition/documentation on hover
* file/workspace symbols
* rename support (?)
* detailed error messages on request
* symbol references
* highlight occurrences
* multi-workspace support (?)
* multiple dhall versions (?)
* snippets
* code completion
* function signatures (?)
* provide import errors source location
* add timeout to requests (throttling?), cancellation of requests

