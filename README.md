# Opt Package Manager

The *Opt Package Manager* is a simple package manager, which installs 
differrent programms under `/opt/`. This is needed, if you want to
use packages, which are not supported by your linux packet manager yet.
E.g. if you need the newest git-version.

## Supported packages

* git

## Install

```
git clone git@github.com:boldt/opm.git
cd opm
```

Add `PATH=/opt/opm/bin:$PATH` to your `.bash_aliases`

### Install git

```
./opm i git 1.8.4.1
```

## Tested with

* Ubuntu 12.04.3

