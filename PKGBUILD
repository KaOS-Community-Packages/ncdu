pkgname=ncdu
pkgver=2.1.2
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("https://dev.yorhel.nl/download/${pkgname}-${pkgver}-linux-x86_64.tar.gz")
sha256sums=('c837b535a5b42b5c9813bc5719358d6fc84ded3c4d477e779edd0f4ca88b2b60')

package() {
	install -Dm755 "${srcdir}/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}
