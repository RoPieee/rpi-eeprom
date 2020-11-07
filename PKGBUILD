# Maintainer: Harry ten Berge <htenberge@gmail.com>

pkgname=rpi-eeprom
pkgver=20201107
pkgrel=1
arch=(any)
url="https://github.com/RoPieee/rpi-eeprom"
license=('custom')
source=('checkout::git+https://github.com/RoPieee/rpi-eeprom.git')
options=(!strip)



package() {
   echo "package"

   install -d -m 755 "${pkgdir}/usr/bin"
   install -D -m 755 checkout/firmware/vl805    "${pkgdir}/usr/bin/vl805"
   install -D -m 755 checkout/rpi-eeprom-config "${pkgdir}/usr/bin/rpi-eeprom-config"
   install -D -m 755 checkout/rpi-eeprom-update "${pkgdir}/usr/bin/rpi-eeprom-update"

   install -d -m 755 "${pkgdir}/usr/lib/firmware/raspberrypi/bootloader"
   cp -r checkout/firmware/* "${pkgdir}/usr/lib/firmware/raspberrypi/bootloader"
}

md5sums=('SKIP')
