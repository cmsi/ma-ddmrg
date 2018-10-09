# ma-ddmrg

DDMRG Debian Package

## How to prepare source files for ddmrg package

```
VERSION=2.0.0
VERSION_MAJOR=$(echo ${VERSION} | cut -d. -f1)
cd $HOME/vagrant/data/src
tar zxvf $HOME/DDMRG${VERSION_MAJOR}.tgz
mv -f DDMRG${VERSION_MAJOR} ddmrg_${VERSION}
tar zcvf ddmrg_${VERSION}.orig.tar.gz ddmrg_${VERSION}
rm -rf ddmrg_${VERSION}
```
