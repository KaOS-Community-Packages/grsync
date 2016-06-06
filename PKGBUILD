pkgname=grsync
pkgver=1.2.6
pkgrel=1
pkgdesc="GTK GUI for sync"
arch=('x86_64')
url="http://www.opbyte.it/grsync"
license=('GPL')
depends=('gtk2' 'rsync')
makedepends=('gettext' 'intltool')
source=(http://www.opbyte.it/release/grsync-$pkgver.tar.gz)
md5sums=('eb2b39e68a04ea5b9c92bcb7d9401e80')

build() {
cd grsync-$pkgver
./configure --prefix=/usr  --disable-unity
make
}

package() {
cd grsync-$pkgver
make DESTDIR=$pkgdir install
}
