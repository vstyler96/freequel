freequel_sources = [
  'main.vala',
  'window.vala',
]

freequel_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk+-3.0', version: '>= 3.22'),
]

gnome = import('gnome')

freequel_sources += gnome.compile_resources('freequel-resources',
  'freequel.gresource.xml',
  c_name: 'freequel'
)

executable('freequel', freequel_sources,
  vala_args: '--target-glib=2.50',  dependencies: freequel_deps,
  install: true,
)
