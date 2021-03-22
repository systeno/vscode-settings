# vscode-settings
VS Code Settings and Extensions

## Installation

### Settings
To install the settings, you need replace the `settings.json` in your vscode config.
The `settings.json` can be found at: `$HOME/.config/Code/User/settings.json`


### Extensions

To install all of my extensions run: `cat vs_code_extensions_list.txt | xargs -n1 code --install-extension`.

**Note:** Theses extensions also include language specific ones. If you dont some of the extensions, either delete
them from the `vs_code_extensions_list.txt` or install them manually.

### Custom Css

For the custom css to work you need to have the `be5invis.vscode-custom-css` extension installed.
You need to reference the `vscode_custom_styles.css` file in your `settings.json`. 
To do this set `"vscode_custom_css.imports": ["file:///path/to/vscode_custom_styles.css"]` inside the `settings.json` to the desired location. 
I recomend to put the `vscode_custom_styles.css` inside the vscode config folder: `$HOME/.config/Code/vscode_custom_styles.css`.

You also need to give yourself write access to the vscode files: `sudo chown -R $(whoami) /usr/share/code`. The location of you vscode may differ.

**Note:** Since the custom css extension changes some unexpected parts of the programm. VS Code may complain about broken files.
The best way to solve this is to tell vscode not to bother you again :).

### Theme

The theme I am using can be found at: [https://github.com/systeno/atomica](https://github.com/systeno/atomica).
