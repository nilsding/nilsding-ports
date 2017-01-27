# $FreeBSD$

PORTNAME=	ocaml-mm
PORTVERSION=	0.3.0
CATEGORIES=	devel
USE_GITHUB=	yes
GH_ACCOUNT=	savonet savonet:m4
GH_PROJECT=	m4:m4
GH_TAGNAME=	81475c9:m4
GH_SUBDIR=	m4:m4

MAINTAINER=	nilsding@nilsding.org
COMMENT=	OCaml multimedia library

LICENSE=	LGPL21

GNU_CONFIGURE=	yes
USES=		gmake
USE_AUTOTOOLS=  autoconf:env

USE_OCAML=	yes
USE_OCAML_FINDLIB=	yes

pre-configure:
	(cd ${WRKSRC} && sh ./bootstrap)



.include <bsd.port.mk>

