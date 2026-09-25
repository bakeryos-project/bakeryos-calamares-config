pkgname=bakeryos-calamares-config
pkgver=1.1.0
pkgrel=1
pkgdesc="Calamares config for BakeryOS"
url="https://github.com/bakeryos-project/bakeryos-calamares-config"
arch=('any')
license=("GPL-3.0-or-later")
source=()
sha256sums=()
options=(!debug !strip)

prepare() {
    cp -r ../etc "${srcdir}/"
}

package() {
    install -d "${pkgdir}/etc"
    cp -r etc/* "${pkgdir}/etc/"

    install -Dm644 "${startdir}/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}