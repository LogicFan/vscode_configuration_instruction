# Wolfram

## Install Wolfram Engine

1. Download from [here](https://www.wolfram.com/engine/) and install.

2. Activate using account.

## Install Wolfram Language Server

1. Install Wolfram Language Server [plugin](https://github.com/kenkangxgwe/vscode-lsp-wl)

2. Git clone the server file from [here](https://github.com/kenkangxgwe/lsp-wl)

3. Open `wolframscript` and run the following

```wolfram
PacletInstall["CodeParser"]
PacletInstall["CodeInspector"]
PacletInstall["AST", "UpdateSites" -> True]
PacletInstall["Lint", "UpdateSites" -> True]
```

4. Set correct path for the following 

```json
{
    "WolframLanguageServer.WLServerPath": "path/to/lsp-wl",
    "WolframLanguageServer.WolframPath": "path/to/wolfram.exe"
}
```

## Install Wolfram Language Syntax Highlighting

1. Install Wolfram Language [plugin](https://github.com/Shigma/vscode-wl)

## Install Code Runner

1. Install Code Runner [plugin](https://github.com/formulahendry/vscode-code-runner)

2. Set the following configuration

```json
{
    "files.associations": {
        "*.wls": "wolfram"
    },
    "code-runner.executorMap": {
        "wolfram": "wolframscript -file"
    }
}
```

