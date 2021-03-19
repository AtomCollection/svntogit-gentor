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
source=("https://github.com/AtomCollection/gentor/releases/download/1.0/gentor-1.0.tar.gz")
md5sums=('d106e09f82affd51f7f9c4c3bdebd04e')
build() {
  cd "$srcdir/$pkgname"
}
package() {
    cd "$srcdir/$pkgname"
    sudo cp -r gentor.py /usr/bin
    sudo cp -r torngconf /usr/bin
    sudo cp gentor-autostart.service /etc/systemd/system
    sudo systemctl daemon-reload
    sudo mv /usr/bin/gentor.py /usr/bin/gentor
    sudo chmod +x /usr/bin/gentor
}
