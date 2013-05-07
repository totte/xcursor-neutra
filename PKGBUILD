# Maintainer: totte <totte@tott.es>
pkgname=xcursor-neutra
pkgver=1.0.0
pkgrel=1
pkgdesc="Personal modification of the Neutral X11 cursor theme"
arch=("any")
url="http://www.tott.es"
license=("PerlArtistic")
depends=()
source=("https://github.com/totte/xcursor-neutra/archive/master.zip")
sha256sums=("f7435f798fb26da2d6fafe182d2e968ff94b5cc830972464305b27b3cdb35e3e")

package() {
  install -dm755 "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/"$pkgname"-master/source/index.theme "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/"$pkgname"-master/cursors "$pkgdir"/usr/share/icons/Neutra
}
