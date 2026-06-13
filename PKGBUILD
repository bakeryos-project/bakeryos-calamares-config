pkgname=bakery-os-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for Bakery OS"
arch=('any')
license=("GPL-3.0-or-later")

package() {
    find etc -type f -exec install -Dm644 {} "${pkgdir}/{}" \;
}