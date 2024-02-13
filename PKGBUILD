# Maintainer: Aldo Adirajasa Fathoni <aldo dot alfathoni at gmail dot com>
pkgname=volctl
_gitname=volctl
pkgver=0.9.3
pkgrel=1
pkgdesc="Per-application volume control and OSD for Linux desktops."
arch=("all")
url="https://buzz.github.io/volctl/"
license=("GPL")
depends=("python3" "python3-gi" "python3-setuptools" "python3-cairo" "pulseaudio" "desktop-file-utils" "python3-pulsectl")
optdepends=("pavucontrol: mixer support", "ayatana-indicator-application: SNI support")
makedepends=("git")
options=(!emptydirs)
source=("git+https://github.com/buzz/volctl.git#tag=v${pkgver}")
md5sums=("SKIP")

package() {
    cd "${_gitname}"
    python3 setup.py install --root="${pkgdir}/" --optimize=1 --install-layout=deb
}

# vim:set ts=2 sw=2 et:
