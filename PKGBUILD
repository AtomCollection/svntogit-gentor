# Maintainer: Chiheb Bayouli <chihebbayouli@gmail.com>
pkgname=gentor
pkgver=1.0
pkgrel=1
pkgdesc="Utility to make your internet traffic anonymized through Tor network"
arch=(any)
url="https://github.com/AtomCollection/GenTor"
license=('MIT')
depends=(python tor macchanger privoxy net-tools curl systemd)
makedepends=()
source=("https://github.com/AtomCollection/GenTor/files/6170564/$pkgname-$pkgver.tar.gz")
md5sums=('d106e09f82affd51f7f9c4c3bdebd04e'
         '13522759afa912a5bd462728d2b52ca8')
build() {
  cd "$srcdir/$pkgname"
}
package() {
    cd "$srcdir/$pkgname"
    python3 install.py
}
