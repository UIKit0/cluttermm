## Copyright (c) 2009  Openismus GmbH <http://www.openismus.com/>
##
## This file is part of cluttermm.
##
## cluttermm is free software: you can redistribute it and/or modify it
## under the terms of the GNU Lesser General Public License as published
## by the Free Software Foundation, either version 2.1 of the License,
## or (at your option) any later version.
##
## cluttermm is distributed in the hope that it will be useful, but
## WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
## See the GNU Lesser General Public License for more details.
##
## You should have received a copy of the GNU Lesser General Public License
## along with this program.  If not, see <http://www.gnu.org/licenses/>.

lib_LTLIBRARIES = libcluttermm-@CLUTTERMM_API_VERSION@.la

include $(srcdir)/../src/filelist.am
include $(srcdir)/filelist.am
include $(top_srcdir)/build/compile-binding.am

local_cppflags = $(binding_includes) $(binding_cppflags) -DCLUTTERMM_BUILD=1

AM_CPPFLAGS = $(local_cppflags) $(CLUTTERMM_CFLAGS)
AM_CXXFLAGS = $(CLUTTERMM_WXXFLAGS)

libcluttermm_@CLUTTERMM_API_VERSION@_la_SOURCES = $(binding_sources)
libcluttermm_@CLUTTERMM_API_VERSION@_la_LDFLAGS = -no-undefined -version-info $(CLUTTERMM_SO_VERSION)
libcluttermm_@CLUTTERMM_API_VERSION@_la_LIBADD  = $(CLUTTERMM_LIBS)
