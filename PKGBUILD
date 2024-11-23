pkgname=pdfjs
pkgver=4.8.69
pkgrel=1
pkgdesc="PDF reader in javascript"
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('887a6e5f0cda2136daf99cc5ae5fe34581c7bfef2ce64f5c27963d965d88d2c6')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
