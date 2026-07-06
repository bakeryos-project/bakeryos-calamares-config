pkgname=bakeryos-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for BakeryOS"
url="https://gitlab.com/bakeryos/bakeryos-calamares-config"
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

    install -Dm644 "${srcdir}/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}