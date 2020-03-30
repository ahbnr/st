pkgname=st-custom
pkgver=r1097.70f3fec
pkgrel=1
pkgdesc="Suckless terminal with mouse scrollback, gruvbox theme and hack nerd font"
arch=('x86_64')
url="https://st.suckless.org/"
license=('MIT')
provides=('st')
depends=('libx11' 'libxft' 'nerd-fonts-hack')

prepare() {
  cp -R $startdir/* $srcdir || true
}

build() {
  ./build.sh
}

package() {
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -m644 -D LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
