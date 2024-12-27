pkgname=pdfjs
pkgver=4.9.155
pkgrel=1
pkgdesc="PDF reader in javascript"
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('1059ba50947a634a531d0bcbef77532020f43811e7996415f502829ec1cc925f')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
