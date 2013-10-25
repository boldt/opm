# Opt Package Manager

The **Opt Package Manager** (OPM) is a simple package manager, which installs 
differrent programms (often from the sources) to `/opt/`. This is needed, 
if you want to use packages, which are not supported by your linux package 
manager yet. E.g. if you need the newest git-version.

## Supported packages

* [git](http://git-scm.com/)
* java7 (currently, only Java7, 32Bit)

## Install

```
git clone git@github.com:boldt/opm.git
mv opm /opt/
```

If you don't have git, just [click here](https://github.com/boldt/opm/archive/master.zip) to get a of the OPM zip.
Afterwards, you can install git easily with OPM. 

## Use OPM and packages

To be able to use the OPM and the packages installed with OPM, please add `PATH=/opt/opm/bin:$PATH` to your `.bash_aliases`.

## Install package

```
sudo ./opm i {PACKAGE} {VERSION}
```

If more than one version is installed, this command can be used to switch 
between different versions.

### git

Git will be installed by compiling the sources.

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

Java7 will be installed by downloading the ready compiled binaries.

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

We use [Semantic Versioning 2.0.0](http://semver.org/).
