# Plugin: A Bash (or anything) Package Manager

A simple package manager for scripts. That's it!

## Install

``` bash
git clone https://github.com/youngmoney/sh-plugin ~/.plugin
```

Then in your bashrc:

``` bash
. ~/.plugin/plugin init
```

## Usage

For a GitHub repo:

``` bash
plugin install youngmoney/sh-copy-paste-reminder
```

and to remove it:

``` bash
plugin uninstall youngmoney/sh-copy-paste-reminder
```

To see all installed plugins:

``` bash
plugin list
```

And to upgrade them:

``` bash
plugin upgrade
```

or just one:

``` bash
plugin upgrade sh-copy-paste-reminder
```

## Options

Primarily to support multi-architecture builds, plugin will look for a
`PLUGIN_REMOVE_SUFFIX` variable. This is a `:` seperated list of binary
suffixes to remove. For instance:

``` bash
PLUGIN_REMOVE_SUFFIX="-linux-amd64"
```

with a repo that has

``` bash
$ ls bin/
runme-darwin-arm64
runme-linux-amd64
```

will result in the following binaries ending up installed

``` bash
runme
runme-darwin-arm64
runme-linux-amd64
```

where `runme` is a link to `runme-linux-amd64`

## Configuration

There is none!

Plugin can run from any directory (feel free to clone it anywhere and
call init from that location).
