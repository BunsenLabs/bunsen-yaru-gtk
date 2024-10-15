flavours = []

available_flavours = [
  'bark',
  'bark-dark',
  'sage',
  'sage-dark',
]

foreach flavour: available_flavours
  theme_name = meson.project_name() + '-' + flavour
  theme_dir = join_paths(get_option('datadir'), 'themes', theme_name, 'openbox-3')
  src_data = join_paths(flavour + '/' + 'openbox-3' + '/' + 'themerc')
  install_data(src_data, install_dir : theme_dir)
  src_assets = join_paths(flavour + '/' + 'openbox-3')
  src_assets_data = run_command(
        'find', src_assets, '-name', '*.xbm', check: false
        ).stdout().strip().split('\n')
  install_data(src_assets_data, install_dir: theme_dir)
endforeach
