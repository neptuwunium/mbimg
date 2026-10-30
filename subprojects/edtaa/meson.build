project('edtaa','cpp')

cpp = meson.get_compiler('cpp')
args = cpp.get_supported_arguments('-Wno-invalid-utf8')

edtaa_lib = static_library(
    'edtaa',
    'edtaa3func.cpp',
    cpp_args: args,
    include_directories: '.',
)

edtaa_dep = declare_dependency(
    include_directories: '.',
    link_with: edtaa_lib,
)

meson.override_dependency('edtaa', edtaa_dep)
