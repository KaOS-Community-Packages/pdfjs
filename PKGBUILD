pkgname=pdfjs
pkgver=4.7.76
pkgrel=1
pkgdesc="PDF reader in javascript"
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('58bb1a90e03dc197b6a3542e3b1e72a6e26a276b9e397684032d1ef3b3b3593f')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
