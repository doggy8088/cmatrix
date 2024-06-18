# CMatrix

This is a docker image for the cmatrix program. CMatrix is a program that simulates the display from "The Matrix" movie. It is provided as a docker image to allow for easy use of the program without the need to install it on the host system.

This image is based on [defnotgustavom/cmatrix](https://hub.docker.com/r/defnotgustavom/cmatrix).

- Running:

    ```sh
    docker run -it --rm --log-driver none --net none --read-only --cap-drop=ALL willh/cmatrix
    ```

- Keybinds:

    `a` Toggle asynchronous scroll

    `b` Random bold characters

    `B` All bold characters

    `n` Turn off bold characters

    `0` \~ `9` Adjust update speed

    `!` `@` `#` `$` `%` `^` `&` `)` Change the color of the matrix to the corresponding color:

     - `!` -- red
     - `@` -- green
     - `#` -- yellow
     - `$` -- blue
     - `%` -- magenta
     - `^` -- cyan
     - `&` -- white
     - `)` -- black

    `q` Quit the program

- Arguments can also be issued via cmatrix -(word);

    `-a`: Asynchronous scroll

    `-b`: Bold characters on

    `-B`: All bold characters (overrides -b)

    `-f`: Force the linux $TERM type to be on

    `-l`: Linux mode (uses matrix console font)

    `-L`: Lock mode (can be closed from another terminal)

    `-o`: Use old-style scrolling

    `-h`: Print usage and exit

    `-n`: No bold characters (overrides -b and -B, default)

    `-s`: "Screensaver" mode, exits on first keystroke

    `-x`: X window mode, use if your xterm is using mtx.pcf

    `-V`: Print version information and exit\

    `-u delay` (0 - 10, default 2): Screen update delay

    `-C [color]`: Use this color for matrix (default green)

## Links

- [Fun With Cmatrix in Linux](https://itsfoss.com/using-cmatrix/)

## Related projects

- [No More Secrets](https://github.com/bartobri/no-more-secrets)