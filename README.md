# ma-respack

RESPACK Debian Package

## How to prepare source files for respack package

1. ソースファイルの準備 (ホスト上で)

        VERSION=20171018
        cd $HOME/vagrant/data/src
        wget -O - http://www.mns.kyutech.ac.jp/cgi-bin/respack.cgi?f=RESPACK.tar.gz | tar zxvf -
        wget -O manual.pdf http://www.mns.kyutech.ac.jp/cgi-bin/respack.cgi?f=manual.pdf
        mv -f RESPACK-$VERSION-dist respack_$VERSION
	mv -f manual.pdf respack_$VERSION
        rm -f respack_$VERSION/sample/xtapp/TiO2.ort.6x6x6/mk_localcoord-and-sc222/genvesta
        tar zcvf respack_$VERSION.orig.tar.gz respack_$VERSION
	rm -rf respack_$VERSION
