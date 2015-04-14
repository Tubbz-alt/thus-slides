pkgname=ttf-casper-typeface
pkgver=1.0
pkgrel=1
download="casper-${pkgver}-${pkgrel}.zip"
pkgdesc="TTF fort Casper Typeface by Michael Chereda"
arch=('any')
url="http://bit.ly/P6AG8D"
license=("OFL1.1")
depends=('fontconfig' 'xorg-fonts-encodings' 'xorg-font-utils')
install=ttf.install
noextract=("${download}")
source=("${download}::https://dl.dropboxusercontent.com/u/57042481/Casper%20Typface.zip")

package() {
	cd "${srcdir}/"
	unzip ${download}
	install -m755 -d "${pkgdir}/usr/share/fonts/TTF"
	install -m644 ${srcdir}/*.ttf "${pkgdir}/usr/share/fonts/TTF/"
	install -m755 -d "${pkgdir}/usr/share/licenses/$pkgname"
	install -m644 ${srcdir}/OFL.txt "${pkgdir}/usr/share/licenses/$pkgname"
}
md5sums=('SKIP')
