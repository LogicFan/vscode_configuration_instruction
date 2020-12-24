# Octave

## Install Octave

1. Download from [here](https://www.gnu.org/software/octave/download.html) and install.

2. Add `path/to/octave/mingw64/bin` to environment variable `PATH`

## Install Plugin

1. Install Octave Hacking [plugin](https://github.com/apjanke/vscode-octave-hacking)

2. Install Octave Debugger [plugin](https://github.com/paulo-fernando-silva/vscOctaveDebugger.git)

## Install Code Runner

1. Install Code Runner [plugin](https://github.com/formulahendry/vscode-code-runner)

2. Set the following configuration

```json
{
    "files.associations": {
        "*.m": "octave"
    },
    "code-runner.executorMap": {
        "octave": "octave",
    }
}
```