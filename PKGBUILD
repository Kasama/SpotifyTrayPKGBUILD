# Maintainer: Roberto Alegro <robertoaall@gmail.com>
pkgname=spotify-tray
pkgver=1.0
pkgrel=1
pkgdesc="A Spotify wrapper that adds a tray icon to the application"
arch=('x86_64' 'i686')
url="https://github.com/Kasama/SpotifyTray"
license=('MIT')
depends=( 'spotify'
	'python'
	'python-pyqt4'
	'xdotool'
	'playerctl')
makedepends=('git')
provides=('spotify-tray')
source=("$pkgname::git+https://github.com/Kasama/SpotifyTray")
md5sums=('SKIP')

package() {
	cd "${pkgname}"

	install -D "${srcdir}/${pkgname}"/spotify-tray.py "${pkgdir}"/usr/bin/spotify-tray.py
	install -D "${srcdir}/${pkgname}"/spotify-tray.desktop "${pkgdir}"/usr/share/applications/spotify-tray.desktop
}
