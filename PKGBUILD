# Maintainer: David7ce
pkgname=calamares-cfg
_destname1="/etc"
pkgver=23.04
pkgrel=1
pkgdesc="calamares 3.3 Config for ArkSys"
arch=('any')
url="https://github.com/arksys-os/"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-config-dev')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}