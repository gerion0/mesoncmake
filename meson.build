project('mesoncmake', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])

cmake = import('cmake')

sdk = subproject('sdk')
sdk_dir = sdk.get_variable('sdk_dir')

app_opts = cmake.subproject_options()
app_opts.add_cmake_defines({'SDK': '@0@'.format(sdk_dir)})
app = cmake.subproject('app', options: app_opts)


