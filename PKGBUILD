pkgname=alexandra
pkgver=1.5.0
pkgrel=1
pkgdesc="Small, fast, but powerful video library, written in C++ with Qt5"
arch=("x86_64")
url="https://github.com/jeka-js/alexandra"
license=('GPL')
depends=('qt5-base' 'mediainfolib' 'hicolor-icon-theme')
source=("https://github.com/jeka-js/alexandra/releases/download/1.5.0/alexandra_${pkgver}_debian-jessie-amd64.deb")
md5sums=('7fb7462be9ef3b49ba99830f8f0de19e')

package() {
  tar -xJf ${srcdir}/data.tar.xz -C "${pkgdir}"
  chmod -R 755 "$pkgdir/usr"
  rm -r $pkgdir/usr/share/doc
  install -d -m 755 $pkgdir/usr/share/pixmaps
  mv $pkgdir/usr/share/icons/$pkgname.png $pkgdir/usr/share/pixmaps/
}
