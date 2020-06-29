# Kovan Desktop Client

## Introduction

Kovan Desktop Client is a tool to synchronize files from İTÜ Kovan Server
with your computer.

## Download


### Source code

The Kovan Desktop Client is developed in Git. Since Git makes it easy to
fork and improve the source code and to adapt it to your need, many copies
can be found on the Internet, in particular on GitHub. However, the
authoritative repository maintained by the developers is located at
https://github.com/ITUBIDB/kovan-desktop-client.

## Building the source code

## MacOS Building steps

* Clone repo `git clone https://github.com/ITUBIDB/kovan-desktop-client/`
* To build up-to-date version of XCode app, brew and packages tools are needed.
* Add ownCloud repo `brew tap owncloud/owncloud`
* Install qt5 using `brew install qt5`
* Install ownCloud dependencies using `brew install $(brew deps owncloud-client)`
* Install qtkeychain `brew install qtkeychain`

* Init submodules using `cd kovan-desktop-client && sudo git submodule init && sudo git submodule update`
* Create build folder `mkdir client-build && cd client-build`
* Configure cmake options `cmake -DCMAKE_PREFIX_PATH=/usr/local/Cellar/qt/5.15.0 -DCMAKE_INSTALL_PREFIX=~/kovan-desktop-client/build ../`
* `make`
* Kovan.app will be under the folder ./client-build/bin or could be executed using `./Kovan` under ./Kovan.app/Contents/MacOS
* Run `./admin/osx/create_mac.sh ./bin/ .` to generate pkg, it will be under build folder that's created on cmake configuration step

## Windows Building steps

### Steps for Windows build will be added

## Reporting issues and contributing

If you find any bugs or have any suggestion for improvement, please
file an issue at https://yardim.itu.edu.tr Do not
contact the authors directly by mail, as this increases the chance
of your report being lost.

If you created a patch, please submit a [Pull
Request](https://github.com/ITUBIDB/kovan-desktop-client/pulls).

## Maintainers and Contributors

The current maintainers of this repository are:

* Ata Öz <ozata1@itu.edu.tr>

Kovan Desktop Client is developed by the ownCloud community and branded by ITU BIDB for usage of Istanbul Technical University.

Past maintainers:
* 

## License

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful, but
    WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
    or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
    for more details.
