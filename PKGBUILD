# Maintainer: Mirdarthos mirdarthos[at]duck[dot]com

pkgname=my-universal-manjaro-update-helper
pkgver=2.5
pkgrel=1
pkgdesc="A helper for updating Manjaro Linux."
arch=('any')
url="https://github.com/Mirdarthos/manjaro-update-helper"
license=('Apache')
depends=('sudo' 'xclip' 'ncurses' 'pamac-cli' 'pacman' 'inxi' 'meld' 'pacman-mirrors')
optdepends=('timeshift: For creating backups with prior to updating if custom command not specified.'
            'libnotify: For recieving desktop nnotifications')
source=("$pkgname-$pkgver.tar.gz::$url/archive/refs/tags/V$pkgver.tar.gz")
sha256sums=('425e9f663bf568bac23cc0c90c075f529f6a488e8569f7933976a7532d9c9ecf')

package() {
    cd manjaro-update-helper-$pkgver
    install -Dm755 src/usr/bin/mumuh -t "$pkgdir/usr/bin/"
}
