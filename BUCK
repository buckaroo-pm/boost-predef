load('//:subdir_glob.bzl', 'subdir_glob')
load('//:buckaroo_macros.bzl', 'buckaroo_deps')

cxx_library(
  name = 'predef',
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
    ('include/boost', '**/*.h'),
  ]),
  srcs = glob([
    "src/**/*.cpp",
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
