# RepRapFirmware-pkg

Source files to generate the RepRapFirmware Debian package for DSF

Licensed under the terms of the GPLv3.

## Build Instructions

1. In this repo create subdirectories `opt/dsf/sd/firmware`
2. Place firmware binaries in the new `firmware` directory
3. Modify `DEBIAN/changelog` and `DEBIAN/control` according to your needs (replace version)
4. Build the package by running `dpkg-deb --build -Zxz <repo dir> <target dir>`
5. Optionally sign it using `dpkg-sig -k <key> -s builder <deb file>`

