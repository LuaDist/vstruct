# Copyright (C) 2007-2012 LuaDist.
# Created by David Manura
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( vstruct NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

install_lua_module ( vstruct vstruct/init.lua )
install_lua_module ( vstruct.ast vstruct/ast.lua )
install_lua_module ( vstruct.ast.Bitpack vstruct/ast/Bitpack.lua )
install_lua_module ( vstruct.ast.Generator vstruct/ast/Generator.lua )
install_lua_module ( vstruct.ast.IO vstruct/ast/IO.lua )
install_lua_module ( vstruct.ast.List vstruct/ast/List.lua )
install_lua_module ( vstruct.ast.Name vstruct/ast/Name.lua )
install_lua_module ( vstruct.ast.Repeat vstruct/ast/Repeat.lua )
install_lua_module ( vstruct.ast.Root vstruct/ast/Root.lua )
install_lua_module ( vstruct.ast.Table vstruct/ast/Table.lua )
install_lua_module ( vstruct.cursor vstruct/cursor.lua )
install_lua_module ( vstruct.io vstruct/io.lua )
install_lua_module ( vstruct.io.a vstruct/io/a.lua )
install_lua_module ( vstruct.io.b vstruct/io/b.lua )
install_lua_module ( vstruct.io.c vstruct/io/c.lua )
install_lua_module ( vstruct.io.f vstruct/io/f.lua )
install_lua_module ( vstruct.io.i vstruct/io/i.lua )
install_lua_module ( vstruct.io.m vstruct/io/m.lua )
install_lua_module ( vstruct.io.p vstruct/io/p.lua )
install_lua_module ( vstruct.io.s vstruct/io/s.lua )
install_lua_module ( vstruct.io.u vstruct/io/u.lua )
install_lua_module ( vstruct.io.x vstruct/io/x.lua )
install_lua_module ( vstruct.io.z vstruct/io/z.lua )
install_lua_module ( vstruct.io.bigendian vstruct/io/bigendian.lua )
install_lua_module ( vstruct.io.defaults vstruct/io/defaults.lua )
install_lua_module ( vstruct.io.endianness vstruct/io/endianness.lua )
install_lua_module ( vstruct.io.hostendian vstruct/io/hostendian.lua )
install_lua_module ( vstruct.io.littleendian vstruct/io/littleendian.lua )
install_lua_module ( vstruct.io.seekb vstruct/io/seekb.lua )
install_lua_module ( vstruct.io.seekf vstruct/io/seekf.lua )
install_lua_module ( vstruct.io.seekto vstruct/io/seekto.lua )
install_lua_module ( vstruct.lexer vstruct/lexer.lua )
install_lua_module ( vstruct.pack vstruct/pack.lua )
install_lua_module ( vstruct.test vstruct/test.lua )
install_lua_module ( vstruct.test.basic vstruct/test/basic.lua )
install_lua_module ( vstruct.test.common vstruct/test/common.lua )
install_lua_module ( vstruct.test.fp-bigendian vstruct/test/fp-bigendian.lua )
install_lua_module ( vstruct.test.struct-test-gen vstruct/test/struct-test-gen.lua )
install_lua_module ( vstruct.test.fp-littleendian vstruct/test/fp-littleendian.lua )
install_lua_module ( vstruct.unpack vstruct/unpack.lua )

install_doc ( README CHANGES TODO )
install_data ( COPYING )
# LICENSE

add_lua_test ( vstruct/test.lua )
