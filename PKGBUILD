# Maintainer: Zyren <ZyrenV@proton.me>
pkgname=mountssh
pkgver=1.0.0
pkgrel=1
pkgdesc="SSHFS mount utility with profile support, network checks, auto-unmount"
arch=('any')
url="https://github.com/ZyrenVX/mountssh"
license=('MIT')
depends=('sshfs' 'openssh' 'fuse2' 'tree' 'lsof')
source=("git+https://github.com/ZyrenVX/mountssh.git")
sha256sums=('SKIP')  # Replace or use 'SKIP' for local installs

package() {
  cd "$srcdir/mountssh"
  install -Dm755 mountssh "$pkgdir/usr/bin/mountssh"

  install -d "$pkgdir/etc/mountssh"
  echo "# Place default profiles here" > "$pkgdir/etc/mountssh/README"

}

