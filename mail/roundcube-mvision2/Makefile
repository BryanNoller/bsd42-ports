# Created by: Alexey V. Degtyarev
# $FreeBSD$

PORTNAME=	mvision2
PORTVERSION=	2
PORTREVISION=	1
CATEGORIES=	mail
MASTER_SITES=	http://roundcubethemes.net/downloads/ \
		ftp://renatasystems.org/pub/FreeBSD/ports/distfiles/
PKGNAMEPREFIX=	roundcube-
PKGNAMESUFFIX=	${PHP_PKGNAMESUFFIX}

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Theme for RoundCube Web Mail

RUN_DEPENDS=	roundcube${PHP_PKGNAMESUFFIX}>=0.2:mail/roundcube@${PHP_FLAVOR}

USES=		php:flavors
IGNORE_WITH_PHP=80
NO_BUILD=	yes
NO_ARCH=	yes

WWWDIR?=	${PREFIX}/www/roundcube/skins/mvision2_en

SUB_FILES=	pkg-message

post-extract:
	@${FIND} ${WRKDIR} -name "._*" -delete

do-install:
	@${MKDIR} ${STAGEDIR}${WWWDIR}
	cd ${WRKDIR}/mvision2_en && ${PAX} -r -w . \
		${STAGEDIR}${WWWDIR}
	${FIND} ${STAGEDIR}${WWWDIR} -type f -exec ${CHMOD} 0644 {} \;

.include <bsd.port.mk>
