bin_PROGRAMS = dnstracer
dnstracer_SOURCES = dnstracer.c dnstracer-broken.h
man_MANS = dnstracer.8

@NOIPV6_TRUE@AM_CFLAGS= -DNOIPV6

dnstracer.8: dnstracer.pod
	$(PERL2MAN_RULE)
PERL2MAN_RULE = \
	pod2man --release="February 10, 2008" --date="February 10, 2008" --center="General Commands Manual" --section=8 $? > $@
