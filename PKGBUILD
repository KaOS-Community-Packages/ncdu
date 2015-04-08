pkgname=ncdu
pkgver=1.11
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("http://dev.yorhel.nl/download/${pkgname}-${pkgver}.tar.gz")
sha1sums=('8f22d713e6d2b28e1f501eee2bd1e03b55550c8d')

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
