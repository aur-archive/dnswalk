pkgname=dnswalk
pkgver=2.0.2
pkgrel=1
pkgdesc="dnswalk is a DNS debugger" 
url="http://sourceforge.net/projects/dnswalk/" 
license="GPL" 
arch=(i686 x86_64)
depends=('perl-net-dns') 
source=(http://heanet.dl.sourceforge.net/sourceforge/dnswalk/dnswalk-2.0.2.tar.gz) 
build() { 
		cd $startdir/src/ 
		patch -p1 < $startdir/dnswalk.patch
		mkdir -p $startdir/pkg/usr/bin
		mkdir -p $startdir/pkg/usr/man/man1
		mkdir -p $startdir/pkg/usr/share/doc/dnswalk
		cp dnswalk $startdir/pkg/usr/bin
		cp do-dnswalk $startdir/pkg/usr/share/doc/dnswalk
		cp CHANGES $startdir/pkg/usr/share/doc/dnswalk
		cp README $startdir/pkg/usr/share/doc/dnswalk
		cp TODO $startdir/pkg/usr/share/doc/dnswalk
		cp rfc1912.txt $startdir/pkg/usr/share/doc/dnswalk
		cp makereports $startdir/pkg/usr/share/doc/dnswalk
		cp sendreports $startdir/pkg/usr/share/doc/dnswalk
		cp dnswalk.1   $startdir/pkg/usr/man/man1
		cp dnswalk.errors $startdir/pkg/usr/share/doc/dnswalk
	}
md5sums=('62b9302822353fad71d51aefdae1cad1')

