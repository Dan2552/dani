
# Dani - Dan Installer

* clones GitHub repositories and "installs" every binary within in the repo's `bin/` directory
* uses ruby-install to install rubies
* uses homebrew to install otherwise unhandled packages

## Installation

Run the following:

``` bash
bash -c "cd ~ && (git clone https://github.com/Dan2552/dani.git .dani || :) && ~/.dani/lib/sourcing/first-time"
```

Installation will automatically add the binary directories to `$PATH` for bash, zsh and fish. For other shells put the equivalent of:

``` bash
export PATH="$HOME/.dani/bin:$HOME/.dani/install:$PATH"
```

## Usage

```
    dani [COMMAND]

EXAMPLE:
    dani install Dan2552/blah

    # will clone the Dan2552/blah repo from Github and try to determine
    # the path where binaries sit. Any binaries it detects will be
    # added to the $PATH.

COMMAND:
    install, i       Installs a given script 
```
