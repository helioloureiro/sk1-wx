# sK1 3.0

[![Build Status](https://app.travis-ci.com/sk1project/sk1-wx.svg?branch=master)](https://app.travis-ci.com/sk1project/sk1-wx) ![platform](https://img.shields.io/badge/platform-Linux-blue.svg) ![platform](https://img.shields.io/badge/platform-Windows-blue.svg) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

<center>

![sK1 3.0 under Ubuntu 21.10

</center>

sK1 3.0 is a cross-platform open source vector graphics editor similar to CorelDRAW, 
Adobe Illustrator, or Freehand. sK1 is oriented for prepress industry, 
so it works with CMYK color space and produces CMYK-based PDF and PS output.

sK1 Project (https://sk1project.net)

### How to install: 

---

* to build package:   `python3 setup.py build`
* to install package:   `python3 setup.py install`
* to remove installation: `python3 setup.py uninstall`

---

* to create source distribution:   `python3 setup.py sdist`

---

* to create binary RPM distribution:  `python3 setup.py bdist_rpm`
* to create binary DEB distribution:  `python3 setup.py bdist_deb`

---

* help on available distribution formats: `python3 setup.py bdist --help-formats`

---


## DETAILS

If you wish testing sK1 you have two installation ways. 
First option is a distutils install with commands:
```
python3 setup.py build
python3 setup.py install
```
But this way is not recommended. The most preferred option is a package 
installation (deb or rpm). You can create package using command:
```
python3 setup.py bdist_deb (for Ubuntu|Mint|Debian etc.)
python3 setup.py bdist_rpm (for Fedora|OpenSuse|Mageia etc.)
```
By installing the package you have full control over all the installed files 
and can easily remove them from the system (it's important for application
preview).

### Dependencies

For successful build either distutils or deb|rpm package you need installing
some development packages. We describe dev-packages for Ubuntu|Debian, but for
other distros they have similar names. So, you need:
```
git
gettext
curl
libcairo2-dev
liblcms2-dev
libmagickwand-dev
libpango1.0-dev
python3-dev
python3-cairo-dev
python3-distutils
python3-distro
```

To run application you need installing also:
```
python3-wxgtk4.0
python3-pil 
python3-reportlab
python3-cairo
python3-cups
```

Also the project depends on several subprojects: `uniconvertor`, `wal`, `build-utils`. You don't need to clone these sources manualy because `setup.py` does it for you automatically.

