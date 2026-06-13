pkgname=bakery-os-calamares-config
pkgver=1.0.0
pkgrel=1
pkgdesc="Calamares config for Bakery OS"
arch=('any')
license=("GPL-3.0-or-later")

package() {
    echo "Current directory: $(pwd)"
    find . -maxdepth 3 -not -path '*/.*'
    ls -R ..

    if [ -d "etc" ]; then
        mkdir -p "${pkgdir}/etc"
        cp -r etc/* "${pkgdir}/etc/"
    else
        echo "Not found"
    fi
}