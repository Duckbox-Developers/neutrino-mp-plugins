AM_CPPFLAGS = \
	@FREETYPE_CFLAGS@ \
	-I$(top_builddir) \
	-I$(top_srcdir)/include

noinst_PROGRAMS = tuxcom

tuxcom_SOURCES = tuxcom.c

tuxcom_LDADD = \
	@FREETYPE_LIBS@

install-exec-local:
	install -d $(DESTDIR)$(PLUGINDIR)
	install -d $(DESTDIR)$(CONFIGDIR)
	install -m 0755 tuxcom $(DESTDIR)$(PLUGINDIR)/tuxcom.so
	install -m 0644 $(srcdir)/tuxcom.cfg $(DESTDIR)$(PLUGINDIR)
	install -m 0644 $(srcdir)/tuxcom_hint.png $(DESTDIR)$(PLUGINDIR)
