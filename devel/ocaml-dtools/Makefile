# $FreeBSD$

PORTNAME=	ocaml-dtools
PORTVERSION=	0.3.2
CATEGORIES=	devel
USE_GITHUB=	yes
GH_ACCOUNT=	savonet savonet:m4
GH_PROJECT=	m4:m4
GH_TAGNAME=	81475c9:m4
GH_SUBDIR=	m4:m4

MAINTAINER=	nilsding@nilsding.org
COMMENT=	OCaml modules for writing daemons

LICENSE=	GPLv2

GNU_CONFIGURE=	yes
USES=		autoreconf gmake

USE_OCAML=	yes
USE_OCAML_FINDLIB=	yes

pre-configure:
	(cd ${WRKSRC} && sh ./bootstrap)

.include <bsd.port.mk>

