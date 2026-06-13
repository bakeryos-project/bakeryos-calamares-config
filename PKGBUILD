pkgname=bakery-os-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for Bakery OS"
arch=('any')
license=("GPL-3.0-or-later")
source=("etc" "LICENSE" "README.md")
sha256sums=('SKIP' 'SKIP' 'SKIP')

prepare() {
    cp -r ../etc "${srcdir}/"
}

package() {
    install -d "${pkgdir}/etc"
    cp -r etc/* "${pkgdir}/etc/"
}