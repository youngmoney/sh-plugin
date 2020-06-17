# Plugin: A Bash (or anything) Package Manager

A simple package manager for scripts. That's it!

## Install

```
git clone https://github.com/youngmoney/sh-plugin ~/.plugin
```

Then in your bashrc:

```
. ~/.plugin/plugin init
```

## Usage

For a GitHub repo:

```
plugin install youngmoney/sh-copy-paste-reminder
```

and to remove it:

```
plugin uninstall youngmoney/sh-copy-paste-reminder
```

To see all installed plugins:

```
plugin list
```

And to upgrade them:

```
plugin upgrade
```

or just one:

```
plugin upgrade sh-copy-paste-reminder
```

## Configuration

There is none!

Plugin can run from any directory (feel free to clone it anywhere and call init from that location).
