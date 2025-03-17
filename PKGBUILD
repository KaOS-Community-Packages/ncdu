pkgname=ncdu
pkgver=2.8
pkgrel=1
pkgdesc='NCurses Disk usage analyzer'
url='http://dev.yorhel.nl/ncdu/'
license=('custom:MIT')
depends=('ncurses')
arch=('x86_64')
source=("https://dev.yorhel.nl/download/${pkgname}-${pkgver}-linux-x86_64.tar.gz")
sha256sums=('3a152145e39325bd9b383c2b192970091c7a618bd93f144ab9d0bcea57960125')

package() {
	install -Dm755 "${srcdir}/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}
