EXTENSION = gp_toolkit
DATA = gp_toolkit--1.0.sql
MODULES =

REGRESS = resource_manager_restore_to_none gp_toolkit resource_manager_switch_to_queue gp_toolkit_resqueue gp_toolkit_ao_funcs

ifdef USE_PGXS
PG_CONFIG = pg_config
PGXS := $(shell $(PG_CONFIG) --pgxs)
include $(PGXS)
else
subdir = gpcontrib/gp_toolkit
top_builddir = ../..
include $(top_builddir)/src/Makefile.global
include $(top_srcdir)/contrib/contrib-global.mk
endif
