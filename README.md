# Visual Studio Code Setup Guide

Note: this is a configuration geared towards mostly JavaScript and Node development.

## Check for new stuff

- [vscodecandothat.com](http://vscodecandothat.com)
- [vscode marketplace](https://marketplace.visualstudio.com/vscode)

## Add JavaScript Support:

Go to "Help > Welcome" and install "JavaScript" support

## Install (the best) Extensions:

- [Prettier](vscode:extension/esbenp.prettier-vscode)
- [Git Lens](vscode:extension/eamodio.gitlens)

## Install the Fira Code font

[Fira Code Font](https://github.com/tonsky/FiraCode)

## Keyboard Shortcuts

- Go Back: `cmd+[`
- Go Forward: `cmd+]`
- uppercase: `cmd+k, cmd+u`
- lowercase: `cmd+k, cmd+l`
- move line down: `ctrl+cmd+down`
- move line up: `ctrl+cmd+up`
- copy line down: `shift+cmd+d`
- discard changes: `cmd+alt+z`

```json
[
  {
    "key": "cmd+[",
    "command": "workbench.action.navigateBack"
  },
  {
    "key": "ctrl+-",
    "command": "-workbench.action.navigateBack"
  },
  {
    "key": "cmd+]",
    "command": "workbench.action.navigateForward"
  },
  {
    "key": "ctrl+shift+-",
    "command": "-workbench.action.navigateForward"
  },
  {
    "key": "cmd+k cmd+u",
    "command": "editor.action.transformToUppercase"
  },
  {
    "key": "cmd+k cmd+l",
    "command": "editor.action.transformToLowercase"
  },
  {
    "key": "ctrl+cmd+down",
    "command": "editor.action.moveLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+down",
    "command": "-editor.action.moveLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+cmd+up",
    "command": "editor.action.moveLinesUpAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+up",
    "command": "-editor.action.moveLinesUpAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "shift+cmd+d",
    "command": "editor.action.copyLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "shift+alt+down",
    "command": "-editor.action.copyLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+cmd+z",
    "command": "git.clean"
  }
]
```

## User Settings:

```json
{
  "workbench.colorTheme": "Visual Studio Dark",
  "editor.formatOnPaste": false,
  "editor.fontFamily": "Fira Code",
  "editor.fontSize": 13,
  "editor.fontLigatures": true,
  "editor.formatOnSave": true,
  "editor.renderWhitespace": "boundary",
  "files.exclude": {
    "**/.git": true,
    "**/.DS_Store": true
  },
  "prettier.singleQuote": true,
  "prettier.eslintIntegration": true,
  "prettier.tabWidth": 2,
  "javascript.implicitProjectConfig.checkJs": false
}
```
