# $FreeBSD$

PORTNAME=	bareos
PORTVERSION=	17.2.5
CATEGORIES=	sysutils
MASTER_SITES=	http://doc.bareos.org/master/
PKGNAMESUFFIX=	-docs
DISTFILES=	${PORTNAME}-manual-main-reference.pdf

MAINTAINER=	acm@FreeBSD.org
COMMENT=	Bareos document set (PDF)

NO_BUILD=	yes

PORTDOCS=	*.pdf

OPTIONS_DEFINE=	DOCS

do-extract:
	${MKDIR} ${WRKSRC}
	${CP} ${DISTDIR}/${PORTNAME}-manual-main-reference.pdf ${WRKSRC}

do-install:
	${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/${PORTNAME}-manual-main-reference.pdf ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
