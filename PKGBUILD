pkgname=rebornos-mirrorlist
pkgver=20241016
pkgrel=1
pkgdesc="RebornOS mirror list for use by pacman"
arch=('any')
url="https://github.com/RebornOS-Team/rebornos-mirrorlist"
license=('GPL3')
source=("reborn-mirrorlist")
backup=("etc/pacman.d/reborn-mirrorlist")
sha256sums=('fbd4b124073d10ff9e4a0f783ea019ad5ad71fd5eca989dc8b13fd11bbd50b4c')

pkgver() {
  date +%Y%m%d
}

package() {
  mkdir -p "$pkgdir/etc/pacman.d"
  install -m644 "$srcdir/reborn-mirrorlist" "$pkgdir/etc/pacman.d/"
}
