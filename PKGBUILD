pkgname=bakery-os-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for Bakery OS"
arch=('any')
license=("GPL-3.0-or-later")
source=("LICENSE" "README.md")
sha256sums=('SKIP' 'SKIP')

pkgver() {
    git describe --long --tags --always | sed 's/^v//;s/\([^-]*-g\)/r\1/;s/-/./g'
}

prepare() {
    cp -r ../etc "${srcdir}/"
}

package() {
    install -d "${pkgdir}/etc"
    cp -r etc/* "${pkgdir}/etc/"
}