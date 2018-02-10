Setup Go
========

This is how I setup my Go development environment on OSX.

Steps
-----

For OSX, `brew install golang`

`mkdir ~/go`

Add environmental variables to your profile (e.g. `~/.bash_profile`):

    export GOPATH="$HOME/go"
    export PATH="$PATH:$HOME/go/bin"

Setup Git to support private repos (use `ssh` instead of `https`):

    git config --global url."git@github.com:".insteadOf "https://github.com/"
    
Install golint

    go get -u github.com/golang/lint/golint

Setup Atom Editor

    cd ~/go
    atom      # this loads Atom with Go env vars

    # install `go-plus` plugin

Setup go dep

    go get -u github.com/golang/dep/cmd/dep
