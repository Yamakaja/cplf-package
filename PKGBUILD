# $Id$
# Maintainer: Yamakaja <yamakaja@yamakaja.me>

pkgname=cplf
pkgver=1.0.0
pkgrel=0
pkgdesc='Compact Packet Log Format Viewer'
arch=('x86_64')
url='https://github.com/Yamakaja/cplf'
license=('MIT')
depends=()
backup=()
makedepends=('gcc')
optdepends=()
validpgpkeys=() # Netfilter Core Team
# 2016-11-03: https sources download is broken with curl
source=('https://github.com/Yamakaja/cplf/archive/master.tar.gz')
md5sums=('SKIP')

prepare() {
:
}

build() {
  cd cplf-master
  ./build.sh
}

package() {
  cd cplf-master
  install -Dm755 cplf "$pkgdir/usr/bin/cplf"
}

# vim:set ts=2 sw=2 et:
