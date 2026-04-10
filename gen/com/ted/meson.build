# Generated file; do not modify.
subdir('Oshi')

sdbusplus_current_path = 'com/ted'

generated_markdown += custom_target(
    'com/ted/Oshi__markdown'.underscorify(),
    input: [
        '../../../yaml/com/ted/Oshi.interface.yaml',
    ],
    output: ['Oshi.md'],
    depend_files: sdbusplusplus_depfiles,
    command: [
        sdbuspp_gen_meson_prog,
        '--command',
        'markdown',
        '--output',
        meson.current_build_dir(),
        '--tool',
        sdbusplusplus_prog,
        '--directory',
        meson.current_source_dir() / '../../../yaml',
        'com/ted/Oshi',
    ],
    install: should_generate_markdown,
    install_dir: [inst_markdown_dir / sdbusplus_current_path],
    build_by_default: should_generate_markdown,
)

