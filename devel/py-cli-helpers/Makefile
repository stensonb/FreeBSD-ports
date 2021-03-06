# Created by: Po-Chuan Hsieh <sunpoet@FreeBSD.org>
# $FreeBSD$

PORTNAME=	cli-helpers
PORTVERSION=	1.1.0
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	cli_helpers-${PORTVERSION}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Helpers for building command-line apps

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}configobj>=5.0.5:devel/py-configobj@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pygments>=1.6:textproc/py-pygments@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}tabulate>=0.8.2:devel/py-tabulate@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}terminaltables>=3.0.0:textproc/py-terminaltables@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}wcwidth>=0:devel/py-wcwidth@${PY_FLAVOR}

USES=		python
USE_PYTHON=	autoplist concurrent distutils

NO_ARCH=	yes

.include <bsd.port.pre.mk>

.if ${PYTHON_REL} < 3000
RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}backports.csv>=1.0.0:devel/py-backports.csv@${PY_FLAVOR}
.endif

.include <bsd.port.post.mk>
