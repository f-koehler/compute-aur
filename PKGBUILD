# Maintainer: Your Name <fabian2804@googlemail.com>
pkgname=boost-compute-git
pkgver=1
pkgrel=1
pkgdesc=""
arch=(i686 x86_64)
url="https://github.com/kylelutz/compute"
license=('boost')
groups=()
depends=()
makedepends=(git cmake boost)
optdepends=()
provides=('boost-compute')
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=('https://github.com/kylelutz/compute.git')
noextract=()
sha256sums=('skip') #autofill using updpkgsums

build() {
  cd "$pkgname-$pkgver"
  mkdir build
  cd build
  cmake ..
  make
  cd ..
}

package() {
  cd "$pkgname-$pkgver"

  make DESTDIR="$pkgdir/" install
}
