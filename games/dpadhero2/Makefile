# $OpenBSD: Makefile.template,v 1.75 2016/03/20 17:19:49 naddy Exp $

PKG_ARCH =	*

COMMENT =	NES rhythm game

V =		20100516
DISTNAME =	dpadhero2
PKGNAME =	dpadhero2-$V

CATEGORIES =	games

HOMEPAGE =	http://dpadhero.com/

MAINTAINER =	Anthony J. Bentley <anthony@anjbe.name>

# Freely downloadable
PERMIT_PACKAGE_CDROM =	No resale grant
PERMIT_PACKAGE_FTP =	Yes

MASTER_SITES =		http://www.dpadhero.com/releases/$V/

EXTRACT_SUFX =		.zip

NO_BUILD =		Yes
NO_TEST =		Yes

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/roms/nes
	${INSTALL_DATA} ${WRKDIR}/dpadhero2.nes ${PREFIX}/share/roms/nes

.include <bsd.port.mk>
