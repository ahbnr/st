pkgname=st-mscrollback-hack-nerd
pkgver=r1094.9bb517b
pkgrel=1
pkgdesc="Suckless terminal with mouse scrollback, gruvbox theme and hack nerd font"
arch=('x86_64')
url="https://st.suckless.org/"
license=('MIT')
depends=('libx11' 'libxft')

prepare() {
  cp -R ./* "$srcdir"
}

build() {
  ./build.sh
}

package() {
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -m644 -D LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
