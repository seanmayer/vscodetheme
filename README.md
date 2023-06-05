# VSCode Custom Theme

![image](https://github.com/seanmayer/vscodetheme/assets/22813313/a63ce185-9c9b-495c-ab1b-6187d1fef1ca)

# How to Change Terminal Style in Visual Studio Code (VSCode)

Follow these steps to change font size, font family, and background color in the terminal.

## 1. Open VSCode settings

You can open the settings by using the shortcut `Ctrl+,` or by navigating through the menu `File -> Preferences -> Settings`.

## 2. Custom Color Settings (Advanced)

If you need more control over your terminal's appearance, you can modify specific elements directly in the `settings.json` file:

```
{
    "editor.inlineSuggest.enabled": true,
    "workbench.sideBar.location": "right",
    "workbench.colorTheme": "GitHub Dark Dimmed",
    "workbench.iconTheme": "vscode-icons",
    "terminal.integrated.defaultProfile.osx": "bash",
    "github.copilot.enable": {
        "*": true,
        "plaintext": false,
        "markdown": true,
        "scminput": false
    },
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": [
                    "source.shell",
                    "string.unquoted.heredoc.shell"
                ],
                "settings": {
                    "foreground": "#93a1a1"
                }
            },
            {
                "scope": [
                    "punctuation.definition.string.begin.shell",
                    "punctuation.definition.string.end.shell"
                ],
                "settings": {
                    "foreground": "#93a1a1"
                }
            }
        ]
    },
    "workbench.colorCustomizations": {    
        "terminal.foreground": "#80a4c2",
        "terminal.background": "#001f3f",
        "terminalCursor.background": "#80a4c2",
        "terminalCursor.foreground": "#80a4c2",
        "terminal.ansiBlack": "#001f3f",
        "terminal.ansiRed": "#85144b",
        "terminal.ansiGreen": "#3D9970",
        "terminal.ansiYellow": "#FFDC00",
        "terminal.ansiBlue": "#0074D9",
        "terminal.ansiMagenta": "#B10DC9",
        "terminal.ansiCyan": "#39CCCC",
        "terminal.ansiWhite": "#AAAAAA",
        "terminal.ansiBrightBlack": "#111111",
        "terminal.ansiBrightRed": "#FF4136",
        "terminal.ansiBrightGreen": "#2ECC40",
        "terminal.ansiBrightYellow": "#FF851B",
        "terminal.ansiBrightBlue": "#7FDBFF",
        "terminal.ansiBrightMagenta": "#F012BE",
        "terminal.ansiBrightCyan": "#7FDBFF",
        "terminal.ansiBrightWhite": "#DDDDDD"
    },
    "terminal.integrated.fontFamily": "Fira Code",
    "terminal.integrated.fontSize": 16
```
Autocompletion to be added for terminal too. https://kubernetes.io/docs/reference/kubectl/cheatsheet/#kubectl-autocomplete
