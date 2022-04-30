pkgname=zram-vam
pkgver=1
pkgrel=1
pkgdesc="zram confs"
depends=('')
arch=('any')

source=("git+https://github.com/Vampire-Offical/zram.git")
sha256sums=('SKIP')


package(){
  cd $srcdir/zram
  install -Dm755 zram.conf $pkgdir/etc/modules-load.d/zram.conf
  install -Dm755 modzram.conf $pkgdir/etc/modprobe.d/zram.conf
  install -Dm755 99-zram.rules $pkgdir/etc/udev/rules.d/99-zram.rules
  install -Dm755 zram.service $pkgdir/etc/systemd/system/zram.service
  install -Dm755 comp_algorithm $pkgdir/sys/block/zram0/comp_algorithm

}

