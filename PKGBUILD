pkgname=ncdu
pkgver=1.14.1
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
makedepends=('clang')
arch=('x86_64')
source=("http://dev.yorhel.nl/download/${pkgname}-${pkgver}.tar.gz")
sha1sums=('143c09158094adbb44f37945b7ba8bb1428862b1')

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
