# Created by: Po-Chuan Hsieh <sunpoet@FreeBSD.org>
# $FreeBSD$

PORTNAME=	graphene-sqlalchemy
PORTVERSION=	2.3.0
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Graphene SQLAlchemy integration

LICENSE=	MIT

RUN_DEPENDS=	${PY_ENUM34} \
		${PYTHON_PKGNAMEPREFIX}graphene>=2.1.3<3:devel/py-graphene@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}promise>=2.3:devel/py-promise@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}six>=1.10.0<2:devel/py-six@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}sqlalchemy13>=1.2<2:databases/py-sqlalchemy13@${PY_FLAVOR}

USES=		python:3.6+
USE_PYTHON=	autoplist concurrent distutils

NO_ARCH=	yes

.include <bsd.port.mk>
