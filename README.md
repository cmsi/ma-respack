<img src="https://ma.issp.u-tokyo.ac.jp/wp-content/themes/materiapps/images/materiapps.svg" width=150>

# MateriApps Debian Package: RESPACK

### RESPACK

RESPACK is a free software of ab initio many-body perturbation codes including calculations for response function with random-phase approximation, Wannier function, and matrix-element evaluations of frequency-dependent screened direct and exchange interactions.

### Version

* 1.1.2-1 (26 Feb 2019)

### Provided packages

* respack

### Target distributions and architectures

* Debian stretch (amd64, i386)
* Debian jessie (amd64, i386)
* Debian wheezy (amd64, i386)

### For users

* How to install RESPACK

  1. Add MateriApps LIVE! apt repository to Debian [[English](https://github.com/cmsi/MateriAppsLive/wiki/UsingMateriAppsInDebian-en)][[日本語](https://github.com/cmsi/MateriAppsLive/wiki/UsingMateriAppsInDebian)]

  2. Install RESPACK
     ```
     suto apt-get install respack
     ```

### For developers

* How to prepare original source tarball

  ```
  VERSION=1.1.2
  wget -O - http://www.mns.kyutech.ac.jp/cgi-bin/respack.cgi?f=RESPACK.tar.gz | tar zxvf -
  wget -O manual.pdf http://www.mns.kyutech.ac.jp/cgi-bin/respack.cgi?f=manual.pdf
  mv -f RESPACK-$VERSION-dist respack_$VERSION
  mv -f manual.pdf respack_$VERSION
  rm -f respack_$VERSION/sample/xtapp/TiO2.ort.6x6x6/mk_localcoord-and-sc222/genvesta
  tar zcvf respack_$VERSION.orig.tar.gz respack_$VERSION
  rm -rf respack_$VERSION
  ```

### Links
  
* [MateriApps LIVE! Home Page](http://cmsi.github.io/MateriAppsLive/)
* [MateriApps LIVE! Forum](https://github.com/cmsi/MateriAppsLive-forum/wiki) (Users Forum)
* [MateriApps LIVE! Wiki](https://github.com/cmsi/MateriAppsLive/wiki) (Documents and FAQ)
* [MateriApps LIVE!](https://ma.issp.u-tokyo.ac.jp/en/app/275) on MateriApps
