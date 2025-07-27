pkgname=pdfjs
pkgver=5.4.54
pkgrel=1
pkgdesc="PDF reader in javascript"
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-dist.zip")
sha256sums=('4257003f79471195fa7c1dafd91e8324f6618e4fc5a95abb922b4c7b9259770a')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
