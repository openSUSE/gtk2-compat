SUBDIRS = m4macros

install-data-local:
	$(MKDIR_P) $(DESTDIR)$(libdir)/pkgconfig
	$(LN_S) gtk+-3.0.pc $(DESTDIR)$(libdir)/pkgconfig/gtk+-2.0.pc
	$(LN_S) gtk+-x11-3.0.pc $(DESTDIR)$(libdir)/pkgconfig/gtk+-x11-2.0.pc
	$(LN_S) gtk+-unix-print-3.0.pc $(DESTDIR)$(libdir)/pkgconfig/gtk+-unix-print-2.0.pc

uninstall-local:
	$(RM) $(DESTDIR)$(libdir)/pkgconfig/gtk+-2.0.pc
	$(RM) $(DESTDIR)$(libdir)/pkgconfig/gtk+-x11-2.0.pc
	$(RM) $(DESTDIR)$(libdir)/pkgconfig/gtk+-unix-print-2.0.pc
