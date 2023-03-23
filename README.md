# hyprland-bumper

Pin and float a window off to the side of the display for reference on [hyprland](https://github.com/hyprwm/Hyprland)


## Installation

Clone this repo

```bash
$ git clone https://github.com/thmsmlr/hyprland-bumper
$ cd hyprland-bumper
$ chmod +x hyprland-bumper
$ ln -s $(realpath hyprland-bumper) /usr/bin/hyprland-bumper
```

Then in your hyprland config, add some keybindings. Mine are:

```
# Grave is the backtick key, same as tilde
bind = $mainMod, Grave, exec, /usr/bin/hyprland-bumper toggle
bind = SHIFT $mainMod, Grave, exec, /usr/bin/hyprland-bumper dock
```


## Why?

I like workspace, but sometimes for a temporary workflow I don't have the muscle
memory to remember which space I put it on. Similarlly too, I like to use my
zero-ith / special workspace for a video I'm watching in the background.

With bumpers I can just keep a window on the side, pull it overtop of the
tiled windows in a single keybinding. This works well with transparent terminal
windows. I commonly use it when i'm doing research and taking notes on my laptop
on the go. It allows me to keep my browser fullscreen while pulling VIM overtop
to take notes without reflowing the browser and messing with the scroll
position.

I also use it while coding. Often I want my code full screen and single
keystroke to pull over a preview window of the website I'm working on while
referencing some of the code underneath. It's pretty common for me to use this
to pop a browser window in and out of the bumper while tweaking CSS of a site.
Or similarly the webserver logs when I get an error.

Really anywhere you'd use a workspace for a single reference window but want to
also reference it with the main window. Bumpers work well for that.
