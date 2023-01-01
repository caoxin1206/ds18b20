from building import *
Import('rtconfig')

src   = []
cwd   = GetCurrentDir()

# add ds18b20 src files.
src += Glob('src/sensor_dallas_ds18b20.c')

src += Glob('sample/ds18b20_sample.c')

# add ds18b20 include path.
path  = [cwd + '/inc']

# add src and include to group.
group = DefineGroup('ds18b20', src, depend = [''], CPPPATH = path)

Return('group')