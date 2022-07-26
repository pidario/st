pkgname=st
pkgver=0.8.5
pkgrel=2
pkgdesc='Simple Terminal'
arch=('x86_64')
depends=(libxft)
url=https://st.suckless.org
license=('MIT')
source=(
  'st'
  'st.desktop'
  'st.1'
  'LICENSE'
  'README'
)
sha256sums=(
  '5ab26b84a13b26e0f22f844ad51442d57e0ca8b4d636d9cc9170038e6ffa4b63'
  '3d0494c3f538013f50d12659b7e0d51b5972ed27c694aafd7af349005d4ef477'
  '5b0d65d135fcc3d51f60e4fe4d86c5bbd1331266f9b38ecfb86914668c03921c'
  'edba5448352eb6f4d56f6a920b31f2bb19177923190a06198ff8c3ec11da7cfa'
  'f767c242485eb537f0df13cbcc182980d29152a6e25036cf65f334fb3ae8b29e'
)
package () {
  bin=$pkgdir/usr/bin
  app=$pkgdir/usr/share/applications
  man=$pkgdir/usr/share/man/man1
  lic=$pkgdir/usr/share/licenses/$pkgname
  doc=$pkgdir/usr/share/doc/$pkgname
  mkdir --parents $bin $app $man $lic $doc
  install -D --mode 0755 st $bin/st
  install -D --mode 0644 st.desktop $app/st.desktop
  install -D --mode 0644 st.1 $man/st.1
  install -D --mode 0644 LICENSE $lic/LICENSE
  install -D --mode 0644 README $doc/README
}
