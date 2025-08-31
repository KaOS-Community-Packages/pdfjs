pkgname=pdfjs
pkgver=5.4.149
pkgrel=1
pkgdesc="PDF reader in javascript"
conflicts=(pdfjs-legacy)
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('a0f6139f8d8de5f62f384b1de899e084f86dceb98b1cd3d8ee0d7bb40b1de541')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
