# $FreeBSD$

PORTNAME=	knewstuff
DISTVERSION=	${KDE_FRAMEWORKS_VERSION}
PORTREVISION=	1
CATEGORIES=	devel kde kde-frameworks

PATCH_SITES=	https://invent.kde.org/frameworks/knewstuff/commit/
PATCHFILES=	243ea6155b28457c8b1441fee8ab1037828d21ba.diff:-p1

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KF5 library for downloading application assets from the network

USES=		cmake compiler:c++11-lib gettext kde:5 qt:5 tar:xz
USE_KDE=	archive attica5 auth codecs completion config \
		configwidgets coreaddons ecm i18n iconthemes itemviews \
		jobwidgets kio kirigami2 package service sonnet textwidgets \
		widgetsaddons windowsystem xmlgui
USE_QT=		concurrent core dbus declarative gui network widgets xml \
		buildtools_build qmake_build

.include <bsd.port.mk>
