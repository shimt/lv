# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Shinichi MOTOKI <shinichi-motoki@overruns.org>
pkgname=lv
pkgver=4.51.8
pkgrel=1
epoch=
pkgdesc="a Powerful Multilingual File Viewer / Grep"
arch=('x86_64')
url="http://www.ff.iij4u.or.jp/~nrt/lv/"
license=('GPL')
groups=()
depends=('ncurses')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("https://github.com/shimt/lv/archive/4.51.8.00.tar.gz")
noextract=()
md5sums=('3be7b8b182ccd96e48989b4e57311193')
validpgpkeys=()

prepare() {
  :
}

build() {
  chmod 755 configure
	./configure --prefix=/usr --libdir=/usr/share --mandir=/usr/share/man
	make
}

check() {
  :
}

package() {
	make DESTDIR="$pkgdir/" install
}
