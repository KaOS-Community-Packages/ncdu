pkgname=ncdu
pkgver=1.14.2
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
makedepends=('clang')
arch=('x86_64')
source=("http://dev.yorhel.nl/download/${pkgname}-${pkgver}.tar.gz")
sha1sums=('f830ff24c6f364627d5697f78c6fa50ab94d0185')

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
