#############################################################################
# Name:        build/cmake/lib/propgrid/CMakeLists.txt
# Purpose:     CMake file for propgrid library
# Author:      Tobias Taschner
# Created:     2016-10-04
# Copyright:   (c) 2016 wxWidgets development team
# Licence:     wxWindows licence
#############################################################################

include(../../source_groups.cmake)

wx_append_sources(PROPGRID_FILES PROPGRID)

wx_add_library(propgrid ${PROPGRID_FILES})
wx_lib_link_libraries(propgrid PRIVATE adv)

wx_finalize_lib(propgrid)
