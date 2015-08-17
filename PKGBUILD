#Author: Alexandre Minoshi(Almin-Soft Group)
#Maintainer: Alexandre Minoshi

pkgname=systemdx-gtk
pkgver=0.11
pkgrel=3
pkgdesc="GUI for systemd. GTK version"
options=('!strip')
arch=('i686' 'x86_64')
url="http://almin-soft.fsay.net/index.php?systemdx"
license=('GPL2')

if [ "${CARCH}" = 'x86_64' ]; then
depends=('gtk3' 'systemd' 'vte' 'lib32-gdk-pixbuf2' 'lib32-gtk2' 'libsystemdx>=0.12-1' 'ssx')
elif [ "${CARCH}" = 'i686' ]; then
depends=('gtk3' 'systemd' 'vte' 'gdk-pixbuf2' 'libsystemdx>=0.12-1' 'ssx')
fi
source=("systemdx_gtk.tar.bz2::http://almin-soft.fsay.net/data/files/systemdx/download.php?get=systemdx_gtk.tar.bz2")

package() {
  install -Dm755 systemdx-gtk $pkgdir/usr/bin/systemdx-gtk
  install -Dm644 systemdx-gtk.desktop $pkgdir/usr/share/applications/systemdx-gtk.desktop
  install -Dm644 systemdxgtk.png $pkgdir/usr/share/pixmaps/systemdxgtk.png
}
md5sums=('447ac55eae2d1501006aaf8eb4aff7e1')
