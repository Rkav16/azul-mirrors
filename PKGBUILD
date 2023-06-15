# Maintainer: Rafael from azul repository

pkgname=azul-mirrors
fname=azul-mirrorlist
pkgver=20230602
pkgrel=1.1
pkgdesc="azul mirrorlist"
arch=('any')
url="https://github.com/azul-repo/azul-mirrors"
license=('GPL3')
source=(${fname})
install=${fname}.install
sha256sums=('52fc89b6ff5bcbce481a216ad755c0b5f2f8e8b73d400b833a367d154ab968f1')

pkgver() {
    date +%Y%m%d
}

package() {
  install -dm755 ${pkgdir}/etc/pacman.d
  install -m644 ${srcdir}/${fname} ${pkgdir}/etc/pacman.d/${fname}-new
}

