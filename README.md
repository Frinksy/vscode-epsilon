# Eclipse Epsilon Languages Extension

Syntax highlighting for the Eclipse Epsilon languages and Emfatic. 

Adapted from the Epsilon extension for Sublime in the Epsilon Labs project: [https://github.com/epsilonlabs/sublime](https://github.com/epsilonlabs/sublime)

## Features

Support is included for the following languages:
- Epsilon Object Language (EOL)
- Epsilon Comparison Language (ECL)
- Epsilon Generation Language (EGL)
- EGL Co-Ordination Language (EGX)
- Epsilon Validation Language (EVL)
- Epsilon Transformation Language (ETL)
- Epsilon Merging Language (EML)
- Epsilon Pattern Language (EPL)
- Epsilon Flock
- Epsilon Pinset
- Flexmi (XML)
- Flexmi (YAML)
- Emfatic

## Epsilon Language Server

Language Server Protocol support is included, using the following language server:  
https://github.com/Frinksy/epsilon-language-server

### Installation

Build the extension:

```sh
npm install
npx @vscode/vsce package
```

You can then install the extension from the generated `.vsix` package.
To do so, you can open the Command Palette in VSCode (usually `Ctrl+Shift+P` or `Cmd+Shift+P`), and run `Extensions: Install from VSIX...`. Alternatively, navigate to the Extensions panel in VSCode, and select `Install from VSIX...` under the `...` submenu ("Views and More Actions").

VSCode may prompt you to reload if it is required.


### Configuration

You should configure the path to the JAR file for the language server. Refer to https://github.com/Frinksy/epsilon-language-server for build instructions.

The configuration key is `epsilon.languageServerPath`. You may also edit these using the Settings UI.
Other configuration keys are available under the `epsilon` namespace, and are discoverable through the Settings UI.

The extension should prompt you to restart the language server on configuration changes.


### Usage

To manually restart the Epsilon Language Server, run the `Epsilon: Restart Epsilon Language Server` command in
the command palette.

