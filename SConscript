from building import *

src     = Glob('*.c')
cwd     = GetCurrentDir()
CPPPATH = [cwd]
LIBS    = []
LIBPATH = []

if GetDepend('SOC_FH8620'):
    LIBS = ['wlan-wiced_gcc']
    LIBPATH = [cwd + '/fh8620']

group = DefineGroup('wlan-wiced', src, depend = ['PKG_USING_WLAN_WICED'], CPPPATH = CPPPATH, LIBS = LIBS, LIBPATH = LIBPATH)

Return('group')
