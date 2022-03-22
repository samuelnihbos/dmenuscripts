# Maintainer: samuelnihbos <samuelnihbos@disroot.org>
pkgname=dmscripts-git
_pkgname=dmscripts
pkgver=1.0.r408.5fd2806
pkgrel=1
pkgdesc="A collection of dmenu scripts (modified ver of distrotube)"
arch=('any')
url="https://github.com/samuelnihbos/dmenuscripts.git"
license=('GPL3')
depends=(dmenu ffmpeg findutils xclip xdotool xorg-xrandr bind jq)
groups=()
makedepends=(pandoc git)
checkdepends=()
optdepends=(
  'emacs'
  'libnotifyt'
  'maim'
  'slock'
  )
provides=(dmenuscripts)
conflicts=(dmenuscripts)
replaces=()
backup=()
options=()
source=("git+$url")
noextract=()
md5sums=('SKIP')
validpgpkeys=()

pkgver() {
  cd "${_pkgname}"
  printf "1.0.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

build() {
  cd "${_pkgname}"
  DESTDIR="$pkgdir/" make clean build
}

package() {
  cd ${_pkgname}
  NAME="${pkgname}" DESTDIR="${pkgdir}/" make install
}

post_install () {
  mandb
}

