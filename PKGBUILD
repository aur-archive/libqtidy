pkgname=libqtidy
_name=libQTidy
pkgver=0.8.7
pkgrel=2
pkgdesc="A Library and some Helper programs that make it easier and more intuitive for Developer to integrate Tidy in Qt Applications."
arch=('i686' 'x86_64')
url="http://qtidy.hjcms.de/"
license=('LGPL2')
depends=('qt4' 'tidyhtml')
makedepends=('make' 'cmake')
source=(ftp://ftp.hjcms.de/QTidy/$pkgver/$_name-$pkgver.tar.bz2)
md5sums=('5c7e4581593ba118faf12342d8be8c98')
build() {
  cd $srcdir/libQTidy-$pkgver
  mkdir build && cd build
  cmake .. || return 1
  make || return 1
  make DESTDIR="$pkgdir/" install || return 1
}
