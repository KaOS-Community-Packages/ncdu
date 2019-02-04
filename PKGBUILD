pkgname=ncdu
pkgver=1.14
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
makedepends=('clang')
arch=('x86_64')
source=("http://dev.yorhel.nl/download/${pkgname}-${pkgver}.tar.gz")
sha1sums=('28c7003ad23d2e3a2d22d2c349bb0c7170752396')

build() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	./configure --prefix=/usr
	make CC=clang
}

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make DESTDIR="${pkgdir}" install
	install -Dm644 COPYING "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
