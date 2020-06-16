# Plugin: A Bash (or anything) Package Manager

A simple package manager for scripts. That's it!

## Install

```
git clone https://github.com/youngmoney/bash-plugin ~/.plugin
```

Then in your bashrc:

```
alias plugin="~/.plugin/plugin"
PATH="~/.plugin/bin:$PATH"
```

## Usage

For a GitHub repo:

```
plugin install youngmoney/bash-copy-paste-reminder
```

and to remove it:

```
plugin install youngmoney/bash-copy-paste-reminder
```

To see all installed plugins:

```
plugin list
```
