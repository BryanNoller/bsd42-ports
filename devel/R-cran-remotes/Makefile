# $FreeBSD$

PORTNAME=	remotes
DISTVERSION=	2.2.0
CATEGORIES=	devel
DISTNAME=	${PORTNAME}_${DISTVERSION}

MAINTAINER=	ygy@FreeBSD.org
COMMENT=	R Package Installation from Remote Repositories, Including 'GitHub'

LICENSE=	GPLv2+

BUILD_DEPENDS=	R-cran-knitr>0:print/R-cran-knitr
TEST_DEPENDS=	R-cran-covr>0:devel/R-cran-covr \
		R-cran-rprojroot>0:devel/R-cran-rprojroot \
		R-cran-testthat>0:devel/R-cran-testthat \
		R-cran-withr>0:devel/R-cran-withr \
		R-cran-curl>0:ftp/R-cran-curl \
		R-cran-knitr>0:print/R-cran-knitr \
		R-cran-brew>0:textproc/R-cran-brew \
		R-cran-rmarkdown>0:textproc/R-cran-rmarkdown

USES=		cran:auto-plist

.include <bsd.port.mk>
