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
sha512sums=('a7aac0cf264c968d50896156730dc0b925045def6e513adf1f2783e19fd1cdd423aa69480963479b95927fb4e863f110f3fc0439661ef7cfcacc7376fe95ff1d')

build() {
cd $pkgname-$pkgver
./configure --prefix=/usr  --disable-unity
make
}

package() {
cd $pkgname-$pkgver
make DESTDIR=$pkgdir install
}
