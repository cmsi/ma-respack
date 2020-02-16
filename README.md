<img src="https://ma.issp.u-tokyo.ac.jp/wp-content/themes/materiapps/images/materiapps.svg" width=150>

# MateriApps Debian Package: RESPACK

### RESPACK

RESPACK is a free software of ab initio many-body perturbation codes including calculations for response function with random-phase approximation, Wannier function, and matrix-element evaluations of frequency-dependent screened direct and exchange interactions.

### Version

* 20200113-1

### Provided packages

* respack

### Target distributions and architectures

* Debian buster (amd64, i386)
* Debian stretch (amd64, i386)
* Debian jessie (amd64, i386)
* Ubuntu xenial (amd64)
* Ubuntu bionic (amd64)

### For users

* How to install RESPACK

  1. Add MateriApps LIVE! apt repository to Debian [[English](https://github.com/cmsi/MateriAppsLive/wiki/UsingMateriAppsInDebian-en)][[日本語](https://github.com/cmsi/MateriAppsLive/wiki/UsingMateriAppsInDebian)]

  2. Install RESPACK
     ```
     suto apt-get install respack
     ```

  3. How to run an example
     ```
     cp -rp /usr/share/respack/sample/xtapp/Al.fcc.6x6x6 .
     cd Al.fcc.6x6x6
     sh Al.sh
     ```

### For developers

* How to prepare original source tarball

  ```
  VERSION=yyyymmdd
  wget -O RESPACK-$VERSION.tar.gz http://www.mns.kyutech.ac.jp/cgi-bin/respack.cgi?f=RESPACK-$VERSION.tar.gz
  tar zxvf RESPACK-$VERSION.tar.gz
  mv -f RESPACK-$VERSION respack_$VERSION
  tar zcvf respack_$VERSION.orig.tar.gz respack_$VERSION
  rm -rf RESPACK-$VERSION.tar.gz respack_$VERSION
  ```

### Links
  
* [MateriApps LIVE! Home Page](http://cmsi.github.io/MateriAppsLive/)
* [MateriApps LIVE! Forum](https://github.com/cmsi/MateriAppsLive-forum/wiki) (Users Forum)
* [MateriApps LIVE! Wiki](https://github.com/cmsi/MateriAppsLive/wiki) (Documents and FAQ)
* [MateriApps LIVE!](https://ma.issp.u-tokyo.ac.jp/en/app/275) on MateriApps
