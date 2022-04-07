pkgname=ncdu
pkgver=2.1.1
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("https://dev.yorhel.nl/download/${pkgname}-${pkgver}-linux-x86_64.tar.gz")
sha256sums=('4a8fdfe634b63b86934bee4e5e6956c9309aab4ef86de08d5fa93be1344c765c')

package() {
	install -Dm755 "${srcdir}/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}
