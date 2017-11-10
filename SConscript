from building import *

src = Glob('*.c')

cwd = GetCurrentDir()

CPPPATH = [cwd]

group = DefineGroup('wlan-wiced', src, depend = [''], CPPPATH = CPPPATH,)

group = group + SConscript('AP6181/SConscript')

Return('group')
