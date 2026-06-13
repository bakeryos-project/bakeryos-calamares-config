pkgname=bakery-os-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for Bakery OS"
arch=('any')
license=('MIT')
depends=('calamares')

package() {
    find etc -type f -exec install -Dm644 {} "${pkgdir}/{}" \;
}