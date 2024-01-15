pkgname=pdfjs
pkgver=4.0.379
pkgrel=1
pkgdesc="PDF reader in javascript"
# conflicts=(pdfjs-legacy)
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('11e5e00cf620e73f4b0b832d662b37d6a0cd25b3d0c817acfffec8516bc922dc')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
