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
sha256sums=("60522d63b08a940078cce665d54654bfd604d36d2134ba7e0872cad52b602ed2")

package() {
  install -dm755 "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/"$pkgname"-master/source/index.theme "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/"$pkgname"-master/cursors "$pkgdir"/usr/share/icons/Neutra
}
