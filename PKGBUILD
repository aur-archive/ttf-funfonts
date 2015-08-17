# Maintainer:  TDY <tdy@archlinux.info>
# Contributor: Ronny Steiner <post@sirsteiner.de>
# Contributor: Darío Andrés Rodríguez <darzephyr@gmail.com>

pkgname=ttf-funfonts
pkgver=2
pkgrel=1
pkgdesc="76 selected TTF fonts from 6760 font packages"
arch=('any')
url="http://thelinuxbox.org/"
license=('custom')
depends=('fontconfig' 'xorg-font-utils')
install=ttf.install
source=(http://thelinuxbox.org/downloads/fonts/${pkgname#*-}.tar.gz
        LICENSE)
md5sums=('3dd9c79d77e58cdb532cc6c21e7914d5'
         'd30e0838c9a9f2a6148bda33b28ad6a6')

package() {
  cd "$srcdir/${pkgname#*-}"
  install -dm755 "$pkgdir/usr/share/fonts/TTF/"
  install -m644 *.ttf "$pkgdir/usr/share/fonts/TTF/"
  install -Dm644 ../LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

# vim:set ts=2 sw=2 et:
