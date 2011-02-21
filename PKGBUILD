# $Id: PKGBUILD 18861 2010-06-16 09:09:52Z spupykin $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Dag Odenhall <dag.odenhall@gmail.com>
# Contributor: Grigorios Bouzakis <grbzks@gmail.com>

pkgname=dwm
pkgver=5.8.2
pkgrel=2
pkgdesc="A dynamic window manager for X"
url="http://dwm.suckless.org"
arch=('i686' 'x86_64')
license=('MIT')
options=(zipman)
depends=('libx11' 'libxinerama')
install=dwm.install
source=(http://dl.suckless.org/dwm/dwm-$pkgver.tar.gz \
	config.h
	dwm.desktop)
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         'f0ba59bf77a53e3a2fc8596740ee5cb8'
         '939f403a71b6e85261d09fc3412269ee')

build() {
  cd $srcdir/$pkgname-$pkgver

  cp $srcdir/config.h config.h

  sed -i 's/CPPFLAGS =/CPPFLAGS +=/g' config.mk
  sed -i 's/CFLAGS =/CFLAGS +=/g' config.mk
  sed -i 's/LDFLAGS =/LDFLAGS +=/g' config.mk

  make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11 || return 1
  make PREFIX=/usr DESTDIR=$pkgdir install || return 1

  install -m644 -D LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE && \
  install -m644 -D README $pkgdir/usr/share/doc/$pkgname/README && \
  install -m644 -D $srcdir/dwm.desktop $pkgdir//etc/X11/sessions/dwm.desktop
}
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '15c7b182e5312c2d6bb1abcd8863ed03'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         'f00cfc6da96a5c7f16ee4711b8f16569'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '2012187e7126c943a4216e50ca414560'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '6d9eb874d239055aa9e0ee5f687f6b63'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '77db7a4bba66bdd01bf09c0d560dbb3d'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '77db7a4bba66bdd01bf09c0d560dbb3d'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '9ab9567e2ce368d64da0ed5e9d95675a'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '9e9c6e7f2475a2ef0863cf56cff2e2d0'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '5af74523026194889f0a156e70fb137e'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '909969ddd2587c907a8c4349cac2e1dc'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         'a17dcd1119c144d9dcd1d2cb95d183e9'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
md5sums=('f0b422bfeaa812d66c6dd15c3cc92a6b'
         '9142e138f31f905c99659921ac596dea'
         '97b5389b1cb8207ac1e9eaaa93b87da4')
