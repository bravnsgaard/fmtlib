project('fmtlib', 'cpp',
  default_options : 'cpp_std=c++17',
  version : '9.0.0')

fmt_inc = include_directories('include')

fmt_lib = static_library('fmt',
  ['src/format.cc', 'src/os.cc'],
  include_directories : fmt_inc)

fmtlib_dep = declare_dependency(
  link_with : fmt_lib,
  include_directories : fmt_inc,
  version : meson.project_version())

