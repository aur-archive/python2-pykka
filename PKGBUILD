# Maintainer: Antoine Pierlot-Garcin <antoine at bokbox dot com>
pkgname=python2-pykka
pkgver=1.2.0
pkgrel=1
pkgdesc="Easy to use concurrency abstractions for Python using the actor model"
arch=('any')
url="http://pykka.readthedocs.org/"
license=('Apache')
depends=('python2')
#makedepends=('')
optdepends=('python2-gevent: Use gevent based actors from pykka.gevent')
provides=('python2-pykka')
conflicts=('python2-pykka-git')
source=("http://pypi.python.org/packages/source/P/Pykka/Pykka-$pkgver.tar.gz")
md5sums=('27cb69507f89e34dc1ff34636c4bc165')

package() {
  cd "$srcdir/Pykka-$pkgver"
  python2 setup.py install --prefix=/usr --root="$pkgdir"/ --optimize=1
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

