load('//:subdir_glob.bzl', 'subdir_glob')
load('//:buckaroo_macros.bzl', 'buckaroo_deps')

cxx_library(
  name = 'oatpp-libressl', 
  header_namespace = 'oatpp-libressl', 
  exported_headers = subdir_glob([
    ('', '*.hpp'), 
    ('', 'client/**/*.hpp'), 
    ('', 'server/**/*.hpp'), 
  ]), 
  srcs = glob([
    '*.cpp', 
    'client/**/*.cpp', 
    'server/**/*.cpp', 
  ]), 
  deps = buckaroo_deps(), 
  visibility = [
    'PUBLIC', 
  ],
)
