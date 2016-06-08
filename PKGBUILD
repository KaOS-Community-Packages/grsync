pkgname=grsync
pkgver=1.2.6
pkgrel=1
pkgdesc="GTK GUI for sync"
arch=('x86_64')
url="http://www.opbyte.it/grsync"
license=('GPL')
depends=('gtk2' 'rsync')
makedepends=('gettext' 'intltool')
source=("http://www.opbyte.it/release/$pkgname-$pkgver.tar.gz")
sha512sums=('')

build() {
cd $pkgname-$pkgver
./configure --prefix=/usr  --disable-unity
make
}

package() {
cd $pkgname-$pkgver
make DESTDIR=$pkgdir install
}
