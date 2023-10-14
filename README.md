micpeek
========

Listen to a pulseaudio mic and plot a live spectrum in the terminal.

![$ micpeek](micpeek.gif)

## Install

```sh
$ pipx install micpeek
```

or

```sh
$ pipx install micpeek@git+https://github.com/pteromys/micpeek.git
```

## Use

Passed a fire truck going the other way and it's making you anxious?
No problem—ssh into the laptop on your desk and just type `micpeek` to
reassure yourself that the fire alarm is not sounding. The gif at the
top of the page is a guy saying some words and whistling some scales,
whereas this is a fire alarm being tested:

![gif of micpeek output when fire alarms are audible](alarmed.gif)

Test it out with your own lovely voice before you use it remotely, so
that you can learn baselines for an empty room or open windows or kids
playing video games. But if you have to, you could validate it remotely
by turning up the volume in `alsamixer` and playing some music.

## Acknowledgements

`micpeek` is built on the
[henrikschnor/pasimple](https://github.com/henrikschnor/pasimple)
pulseaudio python bindings.

Animations were recorded using [asciinema](https://asciinema.org/) in
[Comic Mono](https://dtinth.github.io/comic-mono-font/), converted to
gif with [asciinema/agg](https://github.com/asciinema/agg), and
compressed [with this ffmpeg filter](https://superuser.com/a/556031):

```
split[s0][s1];[s0]palettegen=max_colors=256[p];[s1][p]paletteuse=dither=none
```

## Stalking risk ecosystem impact

Low, I hope. While this example lowers the barrier to entry for hooking
up a laptop mic to arbitrary code, it can't do speech recognition;
and there's creepier stuff out there that's easier to install and use.

Please don't prove me wrong about that, but if you did, please let me
know. :(
