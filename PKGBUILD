pkgname=ncdu
pkgver=1.13
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("http://dev.yorhel.nl/download/${pkgname}-${pkgver}.tar.gz")
sha1sums=('3233c4185208d9989ac528a94817ed92dd59c773')

build() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	./configure --prefix=/usr
	make
}

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make DESTDIR="${pkgdir}" install
	install -Dm644 COPYING "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
