# stargazers-raffle

Run a raffle from the 🌟 stargazers 🌟 of a Github project!

## Overview

It is designed to run directly on Github actions but it can also be used locally on your command line. You need to have a JDK and [scala-cli](https://scala-cli.virtuslab.org/) installed, or you can use the given Nix shell.

The following command makes a binary named `raffle`.

```shell
$ nix-shell
$ scala-cli package . -o raffle -f
```

Run the raffle binary passing two arguments: author and repo name.

```shell
$ ./raffle
Missing expected positional argument!

Usage: stargazers-raffle [] [--show-all-users] <author> <repo>

Stargazers Raffle

Options and flags:
    --help
        Display this help text.
    --version, -v
        Print the version number and exit.
    --show-all-users, -s
        Display all the stargazers before raffle

Environment Variables:
    GH_TOKEN=<string>
        Github personal access token
```
