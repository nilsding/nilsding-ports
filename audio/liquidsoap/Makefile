# $FreeBSD$

PORTNAME=	liquidsoap
PORTVERSION=	1.2.1
CATEGORIES=	audio
USE_GITHUB=	yes
GH_ACCOUNT=	savonet savonet:m4
GH_PROJECT=	m4:m4
GH_TAGNAME=	81475c9:m4
GH_SUBDIR=	m4:m4

MAINTAINER=	nilsding@nilsding.org
COMMENT=	Audio streaming language

LICENSE=	GPLv2

GNU_CONFIGURE=	yes
USES=		autoreconf gmake

USE_OCAML=	yes

SA_DIR=		${LOCALBASE}/${OCAML_SITELIBDIR}
BUILD_DEPENDS=	${SA_DIR}/pcre/pcre.a:devel/ocaml-pcre \
		${SA_DIR}/duppy/duppy.a:devel/ocaml-duppy \
		${SA_DIR}/dtools/dtools.a:devel/ocaml-dtools \
		${SA_DIR}/mm/mm.a:devel/ocaml-mm \
		${SA_DIR}/camomile/camomile.a:devel/ocaml-camomile

pre-configure:
	(cd ${WRKSRC} && sh ./bootstrap)

.include <bsd.port.mk>

