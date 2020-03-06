pkgname=fcitx-table-french
pkgver=0.3.8
pkgrel=1
pkgdesc='French table for Fcitx'
arch=('any')
url=''
license=('GPL')
depends=('fcitx')
makedepends=('cmake' 'intltool')
source=()

build() {
  cmake -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Release .
  make
}

package() {
  make DESTDIR="$pkgdir" install
}
