# bash-prompt
A lightweight (single file), cross-compatible (bash v3/v4, MacOS, Linux) bash prompt.

![Dark Theme](images/dark_theme2.png)

## Features

* Single file installation to keep it simple
* Works on MacOS and Linux (and probably others)
* Multiple color themes that can be switched in the same session
* Text input colorized to emphasize commands being executed
* Easy to modify contents of prompt

## Default Prompt

The included multi-line prompt has the following items:

* Time of day in HH:MM format
* Duration of previous command, colorized to indicate success or failure
* Username, colorized to indicate root or non-root user
* Hostname
* Current path trimmed to three directories (configurable)
* Current git branch if in a git repo
* Number of running/sleeping jobs

## Installation

Download [.bash_prompt](https://github.com/pkazmier/bash-prompt/blob/master/.bash_prompt)
to your $HOME directory. Select a theme from the list below or create your own. Then add
the following block of code to your `$HOME/.bashrc` or `$HOME/.bash_profile`, which will 
ensure the prompt is loaded only during an interactive session.

```bash
if [[ -n $PS1 && -f ~/.bash_prompt ]]; then
  . ~/.bash_prompt
  ps1_dark_theme  # Choose your theme here
fi
```

## Color Themes

Here are the included themes. To switch the theme in your current session, type 
the name of a theme. 

*Note: your colors will vary depending on the ANSI color definitions in your terminal
emulator. I have included my MacOS [Terminal theme](misc/Plastic.terminal) in the
`misc` directory if you want to mimic this exact look. That color theme is based on
Will Stone's [Plastic theme](https://will-stone.github.io/plastic/) for VSCode.*

### Switching Themes
![Switching Theme](images/theme_switching.png)

### ps1_dark_theme
![ps1_dark_theme](images/dark_theme2.png)
![ps1_dark_theme](images/dark_theme.png)

### ps1_colorful_theme
![ps1_colorful_theme](images/colorful_theme2.png)
![ps1_colorful_theme](images/colorful_theme.png)

### ps1_white_theme
![ps1_white_theme](images/white_theme2.png)
![ps1_white_theme](images/white_theme.png)

### ps1_blue_theme
![ps1_blue_theme](images/blue_theme2.png)
![ps1_blue_theme](images/blue_theme.png)

### ps1_green_theme
![ps1_green_theme](images/green_theme2.png)
![ps1_green_theme](images/green_theme.png)

### ps1_yellow_theme
![ps1_yellow_theme](images/yellow_theme2.png)
![ps1_yellow_theme](images/yellow_theme.png)

### ps1_red_theme
![ps1_red_theme](images/red_theme2.png)
![ps1_red_theme](images/red_theme.png)

