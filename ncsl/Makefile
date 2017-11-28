# $OpenBSD$
ONLY_FOR_ARCHS=	amd64

COMMENT=	Tool to count number of code lines in C/C++ program

VERSION=	2.1
DISTNAME=	ncsl-${VERSION}
CATEGORIES=	devel lang
MASTER_SITES=	${HOMEPAGE}/ports/
EXTRACT_SUFX=	.tar.gz

HOMEPAGE=	http://localhost
MAINTAINER=	Nayden Markatchev<nayden@gmail.com>

PERMIT_PACKAGE_FTP=  Yes
PERMIT_PACKAGE_CDROM=  Not known

WANTLIB=	c
MAKE_FILE=	makefile

ALL_TARGET=	ncsl
INSTALL_TARGET=	install_everything

do-install:
	${INSTALL_PROGRAM} ${WRKBUILD}/ncsl ${PREFIX}/bin
	${INSTALL_MAN} ${WRKSRC}/ncsl.1 ${PREFIX}/man/man1

.include <bsd.port.mk>
