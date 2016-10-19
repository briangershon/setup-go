Setup Go
========

This is how I setup my Go development environment.

Steps
-----

Create ~/go

Add environmental variables to your profile (e.g. `.bashrc`):

    export GOPATH="$HOME/go"
    export PATH="$PATH:$HOME/go/bin"

Setup Git to support private repos (use `ssh` instead of `https`):

    git config --global url."git@github.com:".insteadOf "https://github.com/"
