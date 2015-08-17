# Maintainer: Tim Langlois <langlois at cs dot cornell dot edu>
_pkgname=dispy
pkgname=python-$_pkgname
pkgver=3.23
pkgrel=1
pkgdesc="Dispy is a Python framework for parallel execution of computations by distributing them across multiple processors in a single machine (SMP), among many machines in a cluster, grid or cloud."
arch=('any')
url="http://dispy.sourceforge.net/"
license=('MIT')
groups=()
depends=()
makedepends=('setuptools')
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=
source=(https://pypi.python.org/packages/source/d/$_pkgname/$_pkgname-$pkgver.tar.gz)
md5sums=('b3c6b77d151ab4ca9f2bc895d0528ba6')

package_python-dispy() {
  depends+=('python>=3.1')
  cd "$srcdir/$_pkgname-$pkgver"
  python setup.py install --root="$pkgdir/" --optimize=1
}

package_python2-dispy() {
  depends+=('python2>=2.7')
  cd "$srcdir/$_pkgname-$pkgver"
  python setup.py install --root="$pkgdir/" --optimize=1
}

# vim:set ts=2 sw=2 et:
