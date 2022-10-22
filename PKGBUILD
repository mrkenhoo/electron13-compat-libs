pkgname=electron13-compat-libs
pkgver=1.0
pkgrel=0
pkgdesc="Legacy libraries for electron13"
arch=(x86_64)
license=('custom:Copyright OpenJS Foundation and Electron contributors. All rights reserved.')
depends=('electron13')
provides=(libicu{data,i18n,uc}.so.71 libFLAC.so.8)
source=(libFLAC.so.8 libicudata.so.71 libicui18n.so.71 libicuuc.so.71)
sha256sums=('SKIP' 'SKIP' 'SKIP' 'SKIP')

package() {
    [ ! -d "$pkgdir/usr/lib/" ] && mkdir -pv "$pkgdir/usr/lib"
    install -v -m 755 lib* "$pkgdir/usr/lib/"
}
