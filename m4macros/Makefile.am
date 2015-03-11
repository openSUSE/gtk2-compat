m4_GENERATED_FILES = \
	gtk-2.0.m4

m4datadir = $(datadir)/aclocal
m4data_DATA = \
	$(m4_GENERATED_FILES)

gtk-2.0.m4: gtk-2.0.m4.patch gtk-2.0.m4.old1.patch
	for DIR in $$ACLOCAL_PATH $$(if test -f /usr/share/aclocal/dirlist ; then cat /usr/share/aclocal/dirlist ; fi) $$(if test -n "$(ACLOCAL)" ; then $(ACLOCAL) --print-ac-dir ; fi) /usr/share/aclocal ; do \
	if test -f $$DIR/gtk-3.0.m4 ; then \
	cp $$DIR/gtk-3.0.m4 gtk-2.0.m4 ;\
	break ;\
	fi ;\
	done ; \
	if ! patch <$(srcdir)/gtk-2.0.m4.patch ; then \
	rm -f gtk-2.0.m4.orig gtk-2.0.m4.rej ;\
	cp $$DIR/gtk-3.0.m4 gtk-2.0.m4 ;\
	patch <$(srcdir)/gtk-2.0.m4.old1.patch ;\
	fi

EXTRA_DIST = \
	gtk-2.0.m4.patch gtk-2.0.m4.old1.patch

DISTCLEANFILES = \
	$(m4_GENERATED_FILES)
