load('//:subdir_glob.bzl', 'subdir_glob')

prebuilt_cxx_library(
  name = 'predef',
  header_only = True,
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
    ('include/boost', '**/*.h'),
  ]),
  visibility = [
    'PUBLIC',
  ],
)
