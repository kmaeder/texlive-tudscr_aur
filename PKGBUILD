# Maintainer: Kevin Mäder <kmaeder[AT]kevin-maeder[dot]de>
# TU Dresden corporate design classes tudscr by Falk Hanisch

pkgname=texlive-tudscr
pkgver=2.01b
pkgrel=1
pkgdesc="TeX Live - TU Dresden corporate design classes tudscr by Falk Hanisch"
license=('unknown')
arch=('any')
depends=('texlive-core' 'texlive-tudscr-fonts')
url=("http://wwwpub.zih.tu-dresden.de/~fahan/tudscr/")
install=texlive.install
source=("http://wwwpub.zih.tu-dresden.de/~fahan/tudscr/download/download.php?file=bundle/TUD-KOMA-Script_v${pkgver}_Unix_full.zip")
md5sums=('d8bdf2eb7b6650a6148b45452f700039')

TEXPATH=/usr/share/texmf/

package() {
	bsdtar -xf TUD-KOMA-Script_v${pkgver}_Unix_full.zip -C $srcdir
	bsdtar -xf $srcdir/tudscr_v${pkgver}_full.zip
	cd $srcdir
	mkdir -p $pkgdir$TEXPATH
	cp -r doc $pkgdir$TEXPATH
	cp -r tex $pkgdir$TEXPATH
}
