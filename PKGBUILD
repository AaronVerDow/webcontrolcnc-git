pkgname=webcontrolcnc-git
_pkgname=webcontrolcnc
pkgver=0.94
pkgrel=1
pkgdesc="Web interface for Maslow CNC machine."
arch=('x86_64')
url="https://github.com/WebControlCNC/WebControl/"
_tarball="webcontrol-$pkgver-linux-singledirectory.tar.gz"
source_x86_64=("https://github.com/WebControlCNC/WebControl/releases/download/v$pkgver/$_tarball")
sha256sums_x86_64=("539b7e66130e37c79d468c2c6726a41930e1c257c4ca549aa2aca9f0b4b43b7d")
options=(!strip)

package() {
    mkdir -p "$pkgdir/usr/lib"
    cp -r "$srcdir" "$pkgdir/usr/lib/$_pkgname"
    mkdir -p "$pkgdir/etc/systemd/system"
    cp "$srcdir/webcontrolcnc.service" "$pkgdir/etc/systemd/system"
}

