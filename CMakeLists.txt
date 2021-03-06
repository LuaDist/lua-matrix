# Copyright (C) 2007-2012 LuaDist.
# Created by David Manura
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( matrix NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

install_lua_module ( complex lua/complex.lua )
install_lua_module ( matrix lua/matrix.lua )
install_data ( README.txt LICENSE.txt )
install_doc ( doc/complex_changelog.txt doc/fit_changelog.txt doc/matrix_changelog.txt )
install_example ( samples/fit.lua )
install_test ( tests/test_complex.lua )
install_test ( tests/test_fit.lua )
install_test ( tests/test.lua )
install_test ( tests/test_matrix.lua )

add_lua_test ( tests/test.lua )
