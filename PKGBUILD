pkgname=aw-awatcher-bin
pkgver=0.3.1
pkgrel=1
pkgdesc="ActivityWatch-compatible activity and idle watchers, with bundled aw server"
arch=('x86_64')
url="https://github.com/2e3s/awatcher"
license=('MPL-2.0')
depends=("activitywatch")
source=("https://github.com/2e3s/awatcher/releases/download/v0.3.1/aw-awatcher.zip"
        "https://raw.githubusercontent.com/2e3s/awatcher/refs/heads/main/config/aw-awatcher.service")
sha256sums=('b6683c3ac20c6b22ff8c39d576c7bf04be9f183ddcfb7f7e474aceb9aea26b75'
            '7a737c65a197848799140dd3029534eeb01d4cc1711c64fbc130d9e6b850ff8c')

package() {

    mkdir -p $pkgdir/usr/local/bin/
    cp -r aw-awatcher $pkgdir/usr/local/bin/

    mv aw-awatcher.service ~/.config/systemd/user/

}
