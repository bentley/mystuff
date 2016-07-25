# $OpenBSD: Makefile.template,v 1.75 2016/03/20 17:19:49 naddy Exp $

PKG_ARCH =	*

COMMENT =	Game Boy puzzle game

V =		0
PKGNAME =	2048-gb-$V

CATEGORIES =	games

HOMEPAGE =	https://github.com/Sanqui/2048-gb

MAINTAINER =	Anthony J. Bentley <anthony@anjbe.name>

# zlib
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =		http://sanqui.rustedlogic.net/etc/
DIST_SUBDIR =		2048-gb-$V
DISTFILES =		2048.gb

NO_BUILD =		Yes
NO_TEST =		Yes
EXTRACT_ONLY =

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/roms/gb
	${INSTALL_DATA} ${DISTDIR}/${CHECKSUMFILES} ${PREFIX}/share/roms/gb

.include <bsd.port.mk>
