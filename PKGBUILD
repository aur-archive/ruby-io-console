# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Rhys <rhys@johnguant.com>

_gemname=io-console
pkgname=ruby-$_gemname
pkgver=0.4.2
pkgrel=1
pkgdesc='Console interface'
arch=(i686 x86_64)
url='http://www.ruby-lang.org'
license=(ruby)
depends=(ruby)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('0580e983149ce8305278fc52cadcca3912bfa111')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
