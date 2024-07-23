# Makefile for lockout scheduler plugin

AUTOMAKE_OPTIONS = foreign

AM_CXXFLAGS = -fexceptions

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -DSLURM_PLUGIN_DEBUG -I$(top_srcdir) -I$(top_srcdir)/src/common

pkglib_LTLIBRARIES = sched_lockout.la

sched_lockout_la_SOURCES = lockout_wrapper.c	\
			lockout.c	\
			lockout.h
sched_lockout_la_LDFLAGS = $(PLUGIN_FLAGS)
