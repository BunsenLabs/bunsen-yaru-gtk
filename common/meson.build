colorize_dummy_svg = find_program('colorize-dummy-svg.py')
accent_colors_definitions_scss = files('accent-colors.scss.in')[0].full_path()
yaru_colors_defs_scss = files('yaru-colors-defs.scss')[0].full_path()

sass_utils_scss = files([
    'sass-utils.scss',
])

test('sass-utils',
    sassc,
    args: [
        files('test-sass-utils.scss'),
        '/dev/null',
    ])
