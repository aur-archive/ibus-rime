# Maintainer: GONG Chen <chen dot sst at gmail dot com>
# Contributor: 網軍總司令
pkgname=ibus-rime
pkgver=0.9.4
pkgrel=1
pkgdesc="Rime input method engine for ibus"
arch=('i686' 'x86_64')
url="http://code.google.com/p/rimeime/"
license=('GPL3')
depends=('ibus' 'libnotify' 'librime>=0.9.3' 'brise')
makedepends=('cmake')
install=ibus-rime.install
changelog=ChangeLog
source=(http://rimeime.googlecode.com/files/$pkgname-$pkgver.tar.gz)

build() {
  cd "${srcdir}/$pkgname"
  make
}

package() {
  cd "${srcdir}/$pkgname"
  make DESTDIR="$pkgdir" install
}

md5sums=('ec7fdc6f8c772b1c5412be59546bc667')
