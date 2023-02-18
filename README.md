# Linux-RICE

## Introduction

The following repository is a collection of my linux RICE builds. Which comes from inspiration from the r/unixporn sub-reddit. I have also below listed resources which have helped me in forming my current workflow setup and have imporved my overall experience with my persoanl computer. A small recomendation I would give to those who are new to seting up customised linux builds is that their is definitely a learning curve with all of this and a fair amount of theory one should be aware of. I will attempt to give people this theory in the following document.

## My Build

- Manjaro
- BSPWM
- Polybar


## Packages

### Vim

A highly customisable text editor which has been used for decades and is an industry standard in computing.

### Polybar

When using polybar with bspwm one needs to add 

~~~
$HOME/.config/polybar/launch.sh
~~~

into ~/.config/bspwm/bspwmrc

It is also important to creates this "launch.sh" file so that one is able to launch the bar on boot. The contents of this file being...

~~~
#!/bin/bash

# Terminate already running bar instances
killall -q polybar

# Wait until the processes have been shut down
while pgrep -u $UID -x polybar >/dev/null; do sleep 1; done

# Launch Polybar, using default config location ~/.config/polybar/config
polybar mybar &

echo "Polybar launched..."
~~~

### Atom

### Rofi

### BSPWM


