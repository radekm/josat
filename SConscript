
import os

env = Environment(ENV = os.environ)

env.Append(CPPPATH = ['.'])
env.Append(CCFLAGS = '-Wall -D__STDC_FORMAT_MACROS -D__STDC_LIMIT_MACROS -DNDEBUG -O3')

source_files = Split("""
    josat/utils/Options.cc
    josat/utils/System.cc
    josat/core/Solver.cc
    josat/core/Main.cc""")

env.Program('Josat', source_files, LIBS = 'z')
