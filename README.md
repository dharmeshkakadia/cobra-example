cobra-example
=============

An example application built with [cobra](https://github.com/spf13/cobra)

# Steps

1. Install cobra

    `go get github.com/spf13/cobra/cobra`  

2. Initialize cobra-example application
    
    `$GOPATH/bin/cobra init github.com/dharmeshkakadia/cobra-example`

3. Add `hello` and `bye` sub commands to our example app
    
    `$GOPATH/bin/cobra add hello`

    `$GOPATH/bin/cobra add bye`

4. Edit `cmd/hello.go`, `cmd/bye.go` and `main.go` to reflect the command description and logic required.

5. Run `main.go`. You would see full help and subcommands

    ```
    go run main.go

    This application shows how to create modern CLI
    applications in go using Cobra CLI library

    Usage:
    cobra-example [command]

    Available Commands:
    bye         says bye
    hello       says hello
    help        Help about any command

    Flags:
        --config string   config file (default is $HOME/.cobra-example.yaml)
    -h, --help            help for cobra-example
    -t, --toggle          Help message for toggle
    ```