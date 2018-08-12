# Visual Studio Code Setup Guide

Note: this is a configuration geared towards mostly JavaScript and Node development.

## Check for new stuff

- [vscodecandothat.com](vscodecandothat.com)
- [vscode marketplace](https://marketplace.visualstudio.com/vscode)


## Add JavaScript Support:

Go to "Help > Welcome" and install "JavaScript" support


## Install (the best) Extensions:

- [Bookmarks](vscode:extension/alefragnani.Bookmarks)
- [Bracket Colorizer](vscode:extension/CoenraadS.bracket-pair-colorizer)
- [Prettier](vscode:extension/esbenp.prettier-vscode)
- [Git Lens](vscode:extension/eamodio.gitlens)


## Install the Fira Code font

[Fira Code Font](https://github.com/tonsky/FiraCode)


## Keyboard Shortcuts

- Go Back: `cmd-[`
- Go Forward: `cmd-]`
- bookmarks.toggle: `cmd-b`
- uppercase: `cmd-k, cmd-u`
- lowercase: `cmd-k, cmd-l`
- move line down: `ctrl-cmd-down`
- move line up: `ctrl-cmd-up`
- copy line down: `shift-cmd-d`
- discard changes: `cmd-alt-z`

- remove key binding: **Remove Line Comment**

## User Settings:

```json
{
    "workbench.colorTheme": "Visual Studio Light",
    "editor.formatOnPaste": false,
    "editor.fontFamily": "Fira Code",
    "editor.fontSize": 13,
    "editor.fontLigatures": true,
    "editor.formatOnSave": true,
    "editor.renderWhitespace": "boundary",
    "editor.cursorBlinking": "smooth",
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/CVS": true,
        "**/.DS_Store": true,
        "**/.idea": true,
    },
    "prettier.singleQuote": true,
    "prettier.eslintIntegration": true,
    "prettier.tabWidth": 2,
    "bracketPairColorizer.consecutivePairColors": [
        "()",
        "[]",
        "{}",
        [
            "#777",
            "Orange",
            "Blue",
            "SeaGreen",
            "Orchid",
        ],
        "Red"
    ],
    "emmet.triggerExpansionOnTab": true,
    "emmet.includeLanguages": {
        "javascript": "javascriptreact"
    },
    "npm.enableScriptExplorer": true,
    "javascript.implicitProjectConfig.checkJs": false,
}
```
