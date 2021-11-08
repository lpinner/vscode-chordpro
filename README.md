# ChordPro support for Visual Studio Code

This repository contains various elements to support ChordPro files in Visual Studio Code.

It is derived from [sublime-chordpro](https://github.com/kudanai/sublime-chordpro). It includes the following:

 - Syntax highlighting,
 - Snippets
 - Build Systems (chordpro -> PDF) requires ["chordpro"](https://www.chordpro.org) is installed.

## About ChordPro

The ChordPro format is a simple notation syntax for guitar chord and tab files commonly found on the internet.

You can find a more detailed explanation, along with it's origin and history [here](https://www.chordpro.org)

# Installing

- Clone this repo into $HOME/.vscode/extensions

# Setting up chordpro -> PDF conversion
- Store all chordpro files in a folder somewhere
- Open the top level folder, create a .vscode subfolder and copy [tasks.json](https://github.com/lpinner/vscode-chordpro/blob/master/.vscode/tasks.json) into it 
- Ensure you have [chordpro](https://www.chordpro.org/chordpro/chordpro-reference-implementation/) installed and [configured](https://www.chordpro.org/chordpro/chordpro-configuration/) how you like 
- If using Windows, add the folder that `chordpro.exe` is installed into to your `PATH` user environment variable or edit .vscode/tasks.json and replace `"command": "chordpro"` with `"command": "C:\Full\Path\to\chordpro folder\chordpro"` (I don't use Windows so don't know the real installation path)
- When working on chordpro files, open the top level folder in VS Code, not the individual files
- Convert to PDF using Terminal - Run Task... or Terminal - Run Build Task... (ctrl-shift-b)

![tabs](https://user-images.githubusercontent.com/4827816/140823004-197e100f-f10c-4a8b-b68d-1c9f036f488c.png)
 
