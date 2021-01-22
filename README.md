# myst - my simple terminal

This is my custom version of [st](https://st.suckless.org), a simple terminal
emulator for X which sucks less.

It uses the [Nord](https://www.nordtheme.com) theme, an arctic, north-bluish color palette.

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit `config.mk` to match your local setup (st is installed into the
`/usr/local` namespace by default).

Afterwards enter the following command to build and install st (if necessary as
root):

    make clean install

## Running st

If you did not install st with `make clean install`, you must compile the st
terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.
