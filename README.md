micpeek
========

Listen to a pulseaudio mic and plot a live spectrum in the terminal.

## Install

```sh
$ pipx install micpeek@git+https://github.com/pteromys/micpeek.git
```

## Use

Passed a fire truck going the other way and it's making you anxious?
No problem—ssh into the laptop on your desk and reassure yourself that
the fire alarm is not sounding. This is what a guy saying some words
and whistling a scale looks like:

![$ micpeek](micpeek.gif)

And this is what fire alarms look like:

![gif of micpeek output when fire alarms are audible](alarmed.gif)

Test it out with your own lovely voice before you use it remotely, so
that you can learn baselines for an empty room or open windows or kids
playing video games. But if you have to, you could validate it remotely
by turning up the volume in `alsamixer` and playing some music.

## Stalking risk ecosystem impact

Low, I hope. While this example lowers the barrier to entry for hooking
up a laptop mic to arbitrary code, it can't do speech recognition;
and there's creepier stuff out there that's easier to install and use.

Please don't prove me wrong about that, but if you did, please let me
know. :(
