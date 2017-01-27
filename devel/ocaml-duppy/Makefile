# $FreeBSD$

PORTNAME=	ocaml-duppy
PORTVERSION=	0.5.2
CATEGORIES=	devel
USE_GITHUB=	yes
GH_ACCOUNT=	savonet savonet:m4
GH_PROJECT=	m4:m4
GH_TAGNAME=	81475c9:m4
GH_SUBDIR=	m4:m4

MAINTAINER=	nilsding@nilsding.org
COMMENT=	OCaml asynchronous scheduler and monad for server-oriented programming

LICENSE=	LGPL21

GNU_CONFIGURE=	yes
USES=		autoreconf gmake

USE_OCAML=	yes
USE_OCAML_FINDLIB=	yes

SA_DIR=		${LOCALBASE}/${OCAML_SITELIBDIR}
BUILD_DEPENDS=	${SA_DIR}/pcre/pcre.a:devel/ocaml-pcre

pre-configure:
	(cd ${WRKSRC} && sh ./bootstrap)

.include <bsd.port.mk>

