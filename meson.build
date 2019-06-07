project('cmakeBuilder', ['c', 'cpp'])

cm = import('cmake')         # Import the CMake meson module
sp = cm.subproject('cmake')  # Configure the subproject

test('cmakeExe', sp.target('cmake'), args : ['-h'])
