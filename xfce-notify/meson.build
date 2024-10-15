flavours = []

available_flavours = [
  'bark-dark',
  'sage-dark',
]

foreach flavour: available_flavours
  flav = flavour.split('.')
  theme_name = meson.project_name() + '-' + flav[0]
  theme_dir = join_paths(get_option('datadir'), 'themes', theme_name, 'xfce-notify-4.0')
  src_data = flav[0] + '.css'
  install_data(src_data, rename : 'gtk.css', install_dir : theme_dir)
endforeach
