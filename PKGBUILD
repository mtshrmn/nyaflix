# Maintainer: Moshe Sherman <mtshrmn@gmail.com>
pkgname=nyaflix
pkgver="1.0"
pkgrel=1
pkgdesc="Stream anime from the command line"
arch=('any')
depends=('fzf' 'lynx' 'curl' 'peerflix' 'mpv' 'parallel')
optdepends=('noto-fonts-cjk: Chinese, Japanese, and Korean character support'
            'vlc: Use VLC as a media player instead of mpv')
license=('GPL')
url="https://github.com/mtshrmn/nyaflix"
source=("git+https://github.com/mtshrmn/nyaflix.git")
md5sums=('SKIP')
provides=("$pkgname")

build() {
  cd "$srcdir/$pkgname"
  chmod +x nyaflix
}

package() {
  cd "$srcdir/$pkgname"
  install -Dm755 nyaflix "$pkgdir/usr/bin/nyaflix"
  install -Dm644 man/nyaflix.1 "$pkgdir/usr/share/man/man1/nyaflix.1"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  install -Dm644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
}
