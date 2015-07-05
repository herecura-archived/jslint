# Author: Reid Burke <me@reidburke.com>
# Contributor: Douglas Crockford <douglas@crockford.com>
# Contributor: Mikeal Rogers <mikeal.rogers@gmail.com>
# Contributor: Adam Moore
# Contributor: Luke Smith <lsmith@yahoo-inc.com>
# Contributor: Anders Conbere <aconbere@gmail.com>
# Maintainer: reid <me@reidburke.com>
_npmname=jslint
pkgname=nodejs-jslint # All lowercase
pkgver=0.1.9
pkgrel=1
pkgdesc="The JavaScript Code Quality Tool"
arch=(any)
url="https://github.com/reid/node-jslint"
license=(Modified MIT / BSD)
depends=(nodejs)
source=(http://registry.npmjs.org/$_npmname/-/$_npmname-$pkgver.tgz)
noextract=($_npmname-$pkgver.tgz)
sha1sums=(f2699f8fdbbb821d6084a1b222977acf0c88b932)
build() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
# vim:set ts=2 sw=2 et: