# Maintainer: Custom Processing Unlimited <cpunltd[at]gmail[dot]com>
# Contributors: Wey (Archlinux forum user)
pkgname=cafepilot-srm
pkgname1=CafePilot_Service_Request_Monitor
pkgver=2.1.0
pkgrel=3
pkgdesc="CafePilot is a cross-platform (Windows and Linux) client/server software suite that makes managing an Internet cafe of any size a breeze. This is the service request monitor program."
url="http://www.cafepilot.com"
arch=('any')
license=('GPL')
depends=('java-runtime')
# optdepends=('*')
# makedepends=()
# conflicts=()
# replaces=()
# backup=()
# install='*.install'
source=("http://sourceforge.net/projects/cafepilot/files/CafePilot/CafePilot%20Server%20and%20Client/CafePilot_SRM.zip/download"
        "cafepilot-srm.sh")
md5sums=('0952ffd672cabbafc1f4c0a0b2dd16bf'
         '7b68e0499bae1ce854e880f41325fd01')

package() {
  cd "${srcdir}"
  install -Dm755 $pkgname.sh $pkgdir/usr/bin/$pkgname.sh
  install -Dm644 $pkgname1.jar $pkgdir/opt/$pkgname1/$pkgname1.jar
  cp -r "$srcdir"/lib/ "$pkgdir"/opt/$pkgname1/
}

# vim:set ts=2 sw=2 et:
