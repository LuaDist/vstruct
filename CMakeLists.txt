# Copyright (C) 2011 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( vstruct NONE )
cmake_minimum_required ( VERSION 2.6 )
include ( dist.cmake )

install ( DIRECTORY vstruct DESTINATION ${INSTALL_LMOD} )
install_data ( COPYING CHANGES README )

#2DO: Tests .. not sure about this.
