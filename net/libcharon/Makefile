# $FreeBSD$

PORTNAME=	libCharon
DISTVERSION=	4.8.0
CATEGORIES=	net devel cad
DIST_SUBDIR=	Ultimaker

MAINTAINER=	db@FreeBSD.org
COMMENT=	File metadata and streaming library

LICENSE=	LGPL3
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		cmake python:3.4+
STRIP=

USE_GITHUB=	yes
GH_ACCOUNT=	Ultimaker
#GH_TAGNAME=	c34738d

CMAKE_ARGS+=	-DPYTHON_EXECUTABLE:STRING=${PYTHON_CMD} \
		-DPYTHONPREFIX_SITELIBDIR:STRING=${PYTHONPREFIX_SITELIBDIR}
NO_ARCH=	yes

.include <bsd.port.mk>
