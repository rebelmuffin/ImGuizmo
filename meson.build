project('ImGuizmo', 'cpp', version: '1.83', default_options : ['default_library=static'])

imguizmo_includes = include_directories('.')

imgui_dep = dependency('imgui')

sources = [
    'ImCurveEdit.cpp',
    'ImGradient.cpp',
    'ImGuizmo.cpp',
    'ImSequencer.cpp',
    'GraphEditor.cpp',
]

imguizmo_lib = library('ImGuizmo', sources, include_directories : imguizmo_includes, dependencies: [imgui_dep])
imguizmo_dep = declare_dependency(link_with : imguizmo_lib, include_directories : imguizmo_includes)
meson.override_dependency('imguizmo', imguizmo_dep)