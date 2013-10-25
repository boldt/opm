# Opt Package Manager

The **Opt Package Manager** is a simple package manager, which installs 
differrent programms (often from the sources) to `/opt/`. This is needed, 
if you want to use packages, which are not supported by your linux package 
manager yet. E.g. if you need the newest git-version.

## Supported packages

* [git](http://git-scm.com/)
* java7 (atm, only Java7u45, 32Bit)

## Install

```
git clone git@github.com:boldt/opm.git
cd opm
```

Add `PATH=/opt/opm/bin:$PATH` to your `.bash_aliases`

## Install package

```
sudo ./opm i {PACKAGE} {VERSION}
```

If more than one version is installed, this command can be used to switch 
between differnet versions.

### git

#### Install

```
sudo ./opm i git 1.8.4.1
sudo ./opm i git 1.8.4
...
```

#### Remove

```
sudo ./opm r git 1.8.4.1
sudo ./opm r git 1.8.4
...
```

### Java7 (JDK)

#### Install
```
sudo ./opm i java7-32bit 45
sudo ./opm i java7-32bit 40
...
```

#### Remove
```
sudo ./opm r java7-32bit 45
sudo ./opm r java7-32bit 40
...
```

## Tested with

* Ubuntu 12.04.3

## Versioning

We use Semantic [Versioning 2.0.0](http://semver.org/).
