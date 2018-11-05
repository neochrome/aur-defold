# Maintainer: Johan Stenqvist <johan@stenqvist.net>
pkgname=defold
pkgver=1.2.140
pkgrel=1
epoch=
pkgdesc="The ultimate engine for 2D games"
arch=('x86_64')
url="https://www.defold.com/"
license=('custom:Defold')
groups=()
depends=(
	'gtk3'
)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
changelog=
source=(
	"$pkgname-$pkgver.zip::https://d.defold.com/editor2/2fc8ff32c9fa3a16c8f4ce44eba8351c054b33dd/editor2/Defold-x86_64-linux.zip"
	"$pkgname.desktop"
	"LICENSE"
)
noextract=()
sha256sums=('510277193e25b47a938ee6f3d7928fb52ba4506f43d3424bfbfece3573c5ecb1'
            '9e953e3e3a0da31456003cf22cb4c571ca462c2f969ad450cbf26e5af69a79e6'
            '1db60d2d87ed80138acdb9c3deffbbf61ce377f9f411804b7f7ebd5ff9d91325')
validpgpkeys=()
package() {
	mkdir -p "$pkgdir/usr/share"
	cp -r "$srcdir/Defold" "$pkgdir/usr/share/$pkgname"
	chmod -R +r "$pkgdir/usr/share/$pkgname"
	chmod +x "$pkgdir/usr/share/$pkgname/Defold"
	install -Dm644 "$srcdir/$pkgname.desktop" "$pkgdir/usr/share/applications/$pkgname.desktop"
	install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
