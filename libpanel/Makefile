#	$NetBSD: Makefile,v 1.7 2015/11/22 04:30:33 kamil Exp $

WARNS=	4

CPPFLAGS+=	-I${.CURDIR}

LIB=	panel

INCS=	panel.h
INCSDIR=	/usr/include

SRCS=	#

SRCS+=	_deck.c

SRCS+=	above.c
SRCS+=	below.c
SRCS+=	bottom.c
SRCS+=	del.c
SRCS+=	getuser.c
SRCS+=	hidden.c
SRCS+=	hide.c
SRCS+=	move.c
SRCS+=	new.c
SRCS+=	replace.c
SRCS+=	setuser.c
SRCS+=	show.c
SRCS+=	top.c
SRCS+=	update.c
SRCS+=	window.c

LIBDPLIBS+=	curses	${.CURDIR}/../libcurses

MAN=	#
MAN+=	move_panel.3
MAN+=	new_panel.3
MAN+=	panel.3
MAN+=	panel_above.3
MAN+=	panel_hidden.3
MAN+=	panel_userptr.3
MAN+=	update_panels.3

MLINKS+=	new_panel.3 panel_window.3
MLINKS+=	new_panel.3 replace_window.3
MLINKS+=	new_panel.3 replace_panel.3
MLINKS+=	new_panel.3 del_panel.3

MLINKS+=	panel_above.3 top_panel.3
MLINKS+=	panel_above.3 bottom_panel.3
MLINKS+=	panel_above.3 panel_below.3

MLINKS+=	panel_hidden.3 hide_panel.3
MLINKS+=	panel_hidden.3 show_panel.3

MLINKS+=	panel_userptr.3 set_panel_userptr.3

.include <bsd.lib.mk>
