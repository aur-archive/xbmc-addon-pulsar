# Maintainer: M0Rf30

pkgname=xbmc-addon-pulsar
pkgver=0.4.0
pkgrel=3
pkgdesc='Pulsar is an torrent finding and streaming engine for Kodi'
classname=plugin.video.pulsar
arch=('any')
url='https://github.com/steeve/plugin.video.pulsar'
license=('GPL3')
depends=('xbmc')
options=(!strip)
source=("https://github.com/steeve/plugin.video.pulsar/releases/download/v${pkgver}/${classname}-${pkgver}.zip")
install=xbmc-addon-pulsar.install
installpath=usr/share/xbmc/addons/

package() {
  mkdir -p ${pkgdir}/${installpath}
  cp -r ${srcdir}/${classname} ${pkgdir}/${installpath}
  rm ${pkgdir}/${installpath}/${classname}/Makefile
  mkdir ${pkgdir}/${installpath}/repository.pulsar
  rm -r ${pkgdir}/${installpath}/${classname}/resources/bin/{windows_x86,darwin_x64,linux_arm}
}

md5sums=('c2a768067e6c71936c388c3e10f7360a')
