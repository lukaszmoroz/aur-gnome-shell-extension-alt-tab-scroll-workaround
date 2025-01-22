# Maintainer: Łukasz Moroz <lukaszmoroz@gmail.com>

pkgname=gnome-shell-extension-alt-tab-scroll-workaround
pkgver=8
pkgrel=1
pkgdesc="Temporary fix for a bug that buffers the scroll between different windows (e.g., Chrome and VS Code)"
arch=('any')
url="https://github.com/lucasresck/gnome-shell-extension-alt-tab-scroll-workaround"
license=('GPL3')
depends=('gnome-shell')
source=("$pkgname-$pkgver.tar.gz::https://github.com/lucasresck/gnome-shell-extension-alt-tab-scroll-workaround/archive/refs/tags/v$pkgver.tar.gz")
sha512sums=('2204afb84f24d1941b0b6fa73ea640b8c4a915364e4865bb27033eac9172fb0cdb24178b1159cc8562801ab69da9a1c12a6b7e198b6ad3775e1eae0754e1305f')

package() {
    cd "$pkgname-$pkgver"
    _uuid='alt-tab-scroll-workaround@lucasresck.github.io'
    install -Dm644 -t "$pkgdir/usr/share/gnome-shell/extensions/$_uuid" extension.js metadata.json
}
