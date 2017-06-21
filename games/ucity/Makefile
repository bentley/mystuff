# $OpenBSD: Makefile.template,v 1.75 2016/03/20 17:19:49 naddy Exp $

PKG_ARCH =	*

COMMENT =	Game Boy city-building game

V =		1.0
PKGNAME =	ucity-$V

CATEGORIES =	games

HOMEPAGE =	https://github.com/AntonioND/ucity

MAINTAINER =	Anthony J. Bentley <anthony@anjbe.name>

# GPLv3+
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =		https://github.com/AntonioND/ucity/releases/download/v$V/
DIST_SUBDIR =		ucity-$V
DISTFILES =		ucity.gbc

NO_BUILD =		Yes
NO_TEST =		Yes
EXTRACT_ONLY =

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/roms/gb
	${INSTALL_DATA} ${DISTDIR}/${CHECKSUMFILES} ${PREFIX}/share/roms/gb

.include <bsd.port.mk>
