# Maintainer: ldev <ldev@ldev.eu.org>
pkgver=1.0.0
pkgrel=1

pkgname='reltools'
pkgdesc='Collection of tools to make releasing software easier'
arch=('any')
licence=('MIT')

depends=('bash')
makedepends=('git')
source=(
  "git+https://github.com/Xgames123/reltools#commit=$pkgver"
  )
md5sums=('SKIP')

package(){
  cd $pkgname
  mkdir -p "$pkgdir/usr/bin"
  # 755 rwxr-xr-x
  install -Dm 755 "bumppkg" -t "$pkgdir/usr/bin/"
  install -Dm 755 "makepkg_deb" -t "$pkgdir/usr/bin/"
  install -Dm 755 "newaur" -t "$pkgdir/usr/bin/"
}
