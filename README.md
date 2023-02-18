# Linux-RICE

## Introduction

The following repository is a collection of my RICEs. Which comes from inspiration from the r/unixporn sub-reddit, daily using many of these products (to find what works for me). I have also below listed resources which have helped me in forming my current workflow setup and have imporved my overall experience with my persoanl computers. A small recomendation I would give to those who are new to seting up customised UNIX builds is that their is definitely a learning curve with all of this and a fair amount of theory one should be aware of. I will attempt to give people this theory in the following document.

## My Devices and What I Run on Them

TODO

### Thoughts on Choosing a Linux Distro

A interesting place to look for distros is [Distro Watch](https://distrowatch.com/), Where one can see newly released distros and popularity of distros.

As a beginer I would only recommend [Ubuntu](https://ubuntu.com/download/desktop). It by far has the best documentation and community support. If you get stuck you will likely find a solution to the problem you are having online. Overall a great choice.

You can go with more advanced distros like [Arch](https://archlinux.org/download/) and [Gentoo](https://www.gentoo.org/downloads/), to name a few, but these will usually have less forgiving forums on noobies and less documents soltions. The upside being that you learn alot more about how linux works and how computers and OSs work.

## Programs Used By Me

### Vim

A highly customisable text editor which has been used for decades and is an industry standard in computing.

Vim definitely has learning curve and 

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

TODO

### Rofi

TODO

### BSPWM

TODO

