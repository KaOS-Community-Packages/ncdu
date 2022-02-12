pkgname=ncdu
pkgver=2.1
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("https://dev.yorhel.nl/download/${pkgname}-${pkgver}-linux-x86_64.tar.gz")
sha256sums=('a74b4b3632ef281c59a3f0ce74ae6cd7563f544d047f893d303a9ea9ee9b2991')

package() {
	install -Dm755 "${srcdir}/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}
