pkgname=pdfjs
pkgver=4.3.136
pkgrel=1
pkgdesc="PDF reader in javascript"
# conflicts=(pdfjs-legacy)
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('2f454599019418a9a3ebdd4a6483dcf4b76ba6c670571aa26acfb0cab54b397b')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
