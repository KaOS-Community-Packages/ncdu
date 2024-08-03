pkgname=ncdu
pkgver=2.5
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("https://dev.yorhel.nl/download/${pkgname}-${pkgver}-linux-x86_64.tar.gz")
sha256sums=('8dc33f5e9c0e22a25af361173f841c7ee2d7c75601064e979a87fef82338b277')

package() {
	install -Dm755 "${srcdir}/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}
