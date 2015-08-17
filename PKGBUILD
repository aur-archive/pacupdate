# Contributor: Hugo Doria <hugo@archlinux.org>
# Contributor: Jaroslav Lichtblau <dragonlord@aur.archlinux.org>

pkgname=pacupdate
pkgver=0.1.1
pkgrel=4
pkgdesc="A simple update notifier for Arch Linux (pacman)"
arch=('any')
url="http://code.google.com/p/pacupdate/"
license=('GPL2')
depends=('python-notify' 'notification-daemon' 'pygtk>=2.13' 'sudo' 'pacman>=3.2' 'python2>=2.7')
install=pacupdate.install
source=(http://${pkgname}.googlecode.com/files/${pkgname}-${pkgver}.tar.gz)
md5sums=('d68407103e0dd9402034cca9f9d1e447')

package() {
  cd ${srcdir}/${pkgname}-${pkgver}

  make PREFIX=/usr DESTDIR=${pkgdir} PYTHON=`which python2` install
}
