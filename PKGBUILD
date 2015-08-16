# Maintainer: Stefan Tatschner <stefan@sevenbyte.org>

pkgname=mybb-lang-ger
pkgver=1.6.14
pkgrel=1
pkgdesc="German language package"
install=mybb-lang-ger.install
arch=('any')
url=('http://mybb.com')
license=('GPL')
depends=('mybb')
source=("${pkgname}::git+https://github.com/mybboard-de/MyBB-German.git#commit=6857e07d6be45e2a024b44db7fcd6e1ec62d19e5")
md5sums=('SKIP')

package() {
  mkdir -p ${pkgdir}/var/lib/mybb/languages
  mkdir -p ${pkgdir}/usr/share/webapps/mybb/images

  cp -ra ${srcdir}/${pkgname}/lang_deutsch_du/Sprachdateien/* ${pkgdir}/var/lib/mybb/languages/
  cp -ra ${srcdir}/${pkgname}/lang_deutsch_sie/Sprachdateien/* ${pkgdir}/var/lib/mybb/languages/
  cp -ra ${srcdir}/${pkgname}/lang_deutsch_du/Buttons/* ${pkgdir}/usr/share/webapps/mybb/images/
  cp -ra ${srcdir}/${pkgname}/lang_deutsch_sie/Buttons/* ${pkgdir}/usr/share/webapps/mybb/images/
}
