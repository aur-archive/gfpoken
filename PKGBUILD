# $Id: PKGBUILD 7784 2008-08-04 09:40:37Z ronald $
# Maintainer: dale <dale@archlinux.org>
# Contributor: Tom Newsom <Jeepster@gmx.co.uk>

pkgname=gfpoken
pkgver=0.25
pkgrel=1
pkgdesc="GFingerPoken is a black-box type game for gtk 1.2 or higher"
url="http://gfpoken.bigw.org/"
depends=('gtk')
source=(http://gfpoken.bigw.org/$pkgname-$pkgver.tar.gz)
license=('GPL')
arch=('i686' 'x86_64')
md5sums=('59365bf8fd96ae3e231c57da7aa26c03')

build() {
cd $startdir/src/$pkgname-$pkgver
./configure --prefix=/usr
make || return 1
make prefix=$startdir/pkg/usr install
}
