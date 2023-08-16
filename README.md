# Python packaged for Immich Distribution

[Python](https://www.python.org/) is a programming language that I use in [Immich Distribution](https://github.com/nsg/immich-distribution). This repo is used as a dependency of the Immich Distribution project and is not intended for direct consumption.

## Usage

```yaml
stage-snaps:
    - immich-distribution-python/latest/stable
```

## Contents
```
.
├── etc
│   └── fonts
│       ├── conf.avail
│       │   ├── 10-antialias.conf
│       │   ├── 10-autohint.conf
│       │   ├── 10-hinting-full.conf
│       │   ├── 10-hinting-medium.conf
│       │   ├── 10-hinting-none.conf
│       │   ├── 10-hinting-slight.conf
│       │   ├── 10-no-sub-pixel.conf
│       │   ├── 10-scale-bitmap-fonts.conf
│       │   ├── 10-sub-pixel-bgr.conf
│       │   ├── 10-sub-pixel-rgb.conf
│       │   ├── 10-sub-pixel-vbgr.conf
│       │   ├── 10-sub-pixel-vrgb.conf
│       │   ├── 10-unhinted.conf
│       │   ├── 11-lcdfilter-default.conf
│       │   ├── 11-lcdfilter-legacy.conf
│       │   ├── 11-lcdfilter-light.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-lgc-serif.conf
│       │   ├── 20-unhint-small-dejavu-sans.conf
│       │   ├── 20-unhint-small-dejavu-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-serif.conf
│       │   ├── 20-unhint-small-vera.conf
│       │   ├── 25-unhint-nonlatin.conf
│       │   ├── 30-metric-aliases.conf
│       │   ├── 40-nonlatin.conf
│       │   ├── 45-generic.conf
│       │   ├── 45-latin.conf
│       │   ├── 49-sansserif.conf
│       │   ├── 50-user.conf
│       │   ├── 51-local.conf
│       │   ├── 53-monospace-lcd-filter.conf
│       │   ├── 57-dejavu-sans.conf
│       │   ├── 57-dejavu-sans-mono.conf
│       │   ├── 57-dejavu-serif.conf
│       │   ├── 58-dejavu-lgc-sans.conf
│       │   ├── 58-dejavu-lgc-sans-mono.conf
│       │   ├── 58-dejavu-lgc-serif.conf
│       │   ├── 60-generic.conf
│       │   ├── 60-latin.conf
│       │   ├── 65-fonts-persian.conf
│       │   ├── 65-khmer.conf
│       │   ├── 65-nonlatin.conf
│       │   ├── 69-unifont.conf
│       │   ├── 70-force-bitmaps.conf
│       │   ├── 70-no-bitmaps.conf
│       │   ├── 70-yes-bitmaps.conf
│       │   ├── 80-delicious.conf
│       │   └── 90-synthetic.conf
│       ├── conf.d
│       │   ├── 10-antialias.conf -> ../conf.avail/10-antialias.conf
│       │   ├── 10-hinting-slight.conf -> ../conf.avail/10-hinting-slight.conf
│       │   ├── 10-scale-bitmap-fonts.conf -> ../conf.avail/10-scale-bitmap-fonts.conf
│       │   ├── 11-lcdfilter-default.conf -> ../conf.avail/11-lcdfilter-default.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans.conf
│       │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-lgc-serif.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-serif.conf
│       │   ├── 20-unhint-small-dejavu-sans.conf -> ../conf.avail/20-unhint-small-dejavu-sans.conf
│       │   ├── 20-unhint-small-dejavu-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-sans-mono.conf
│       │   ├── 20-unhint-small-dejavu-serif.conf -> ../conf.avail/20-unhint-small-dejavu-serif.conf
│       │   ├── 20-unhint-small-vera.conf -> ../conf.avail/20-unhint-small-vera.conf
│       │   ├── 30-metric-aliases.conf -> ../conf.avail/30-metric-aliases.conf
│       │   ├── 40-nonlatin.conf -> ../conf.avail/40-nonlatin.conf
│       │   ├── 45-generic.conf -> ../conf.avail/45-generic.conf
│       │   ├── 45-latin.conf -> ../conf.avail/45-latin.conf
│       │   ├── 49-sansserif.conf -> ../conf.avail/49-sansserif.conf
│       │   ├── 50-user.conf -> ../conf.avail/50-user.conf
│       │   ├── 51-local.conf -> ../conf.avail/51-local.conf
│       │   ├── 57-dejavu-sans.conf -> ../conf.avail/57-dejavu-sans.conf
│       │   ├── 57-dejavu-sans-mono.conf -> ../conf.avail/57-dejavu-sans-mono.conf
│       │   ├── 57-dejavu-serif.conf -> ../conf.avail/57-dejavu-serif.conf
│       │   ├── 58-dejavu-lgc-sans.conf -> ../conf.avail/58-dejavu-lgc-sans.conf
│       │   ├── 58-dejavu-lgc-sans-mono.conf -> ../conf.avail/58-dejavu-lgc-sans-mono.conf
│       │   ├── 58-dejavu-lgc-serif.conf -> ../conf.avail/58-dejavu-lgc-serif.conf
│       │   ├── 60-generic.conf -> ../conf.avail/60-generic.conf
│       │   ├── 60-latin.conf -> ../conf.avail/60-latin.conf
│       │   ├── 65-fonts-persian.conf -> ../conf.avail/65-fonts-persian.conf
│       │   ├── 65-nonlatin.conf -> ../conf.avail/65-nonlatin.conf
│       │   ├── 69-unifont.conf -> ../conf.avail/69-unifont.conf
│       │   ├── 70-no-bitmaps.conf -> ../conf.avail/70-no-bitmaps.conf
│       │   ├── 80-delicious.conf -> ../conf.avail/80-delicious.conf
│       │   ├── 90-synthetic.conf -> ../conf.avail/90-synthetic.conf
│       │   └── README
│       └── fonts.conf
├── meta
│   └── snap.yaml
└── usr
    ├── lib
    │   ├── tcltk
    │   │   └── x86_64-linux-gnu
    │   │       └── tk8.6
    │   │           └── pkgIndex.tcl
    │   └── x86_64-linux-gnu
    │       ├── libfontconfig.so.1 -> libfontconfig.so.1.12.0
    │       ├── libfontconfig.so.1.12.0
    │       ├── libfreetype.so.6 -> libfreetype.so.6.17.1
    │       ├── libfreetype.so.6.17.1
    │       ├── libgdbm.so.6 -> libgdbm.so.6.0.0
    │       ├── libgdbm.so.6.0.0
    │       ├── libpng16.so.16 -> libpng16.so.16.37.0
    │       ├── libpng16.so.16.37.0
    │       ├── libtcl8.6.so
    │       ├── libtcl8.6.so.0 -> libtcl8.6.so
    │       ├── libtk8.6.so
    │       ├── libtk8.6.so.0 -> libtk8.6.so
    │       ├── libX11.so.6 -> libX11.so.6.3.0
    │       ├── libX11.so.6.3.0
    │       ├── libXau.so.6 -> libXau.so.6.0.0
    │       ├── libXau.so.6.0.0
    │       ├── libxcb.so.1 -> libxcb.so.1.1.0
    │       ├── libxcb.so.1.1.0
    │       ├── libXdmcp.so.6 -> libXdmcp.so.6.0.0
    │       ├── libXdmcp.so.6.0.0
    │       ├── libXext.so.6 -> libXext.so.6.4.0
    │       ├── libXext.so.6.4.0
    │       ├── libXft.so.2 -> libXft.so.2.3.3
    │       ├── libXft.so.2.3.3
    │       ├── libXrender.so.1 -> libXrender.so.1.3.0
    │       ├── libXrender.so.1.3.0
    │       ├── libXss.so.1 -> libXss.so.1.0.0
    │       └── libXss.so.1.0.0
    ├── local
    │   ├── bin
    │   │   ├── 2to3 -> 2to3-3.11
    │   │   ├── 2to3-3.11
    │   │   ├── idle3 -> idle3.11
    │   │   ├── idle3.11
    │   │   ├── pip3
    │   │   ├── pip3.11
    │   │   ├── pydoc3 -> pydoc3.11
    │   │   ├── pydoc3.11
    │   │   ├── python3 -> python3.11
    │   │   ├── python3.11
    │   │   ├── python3.11-config
    │   │   └── python3-config -> python3.11-config
    │   ├── include
    │   │   └── python3.11
    │   │       ├── abstract.h
    │   │       ├── bltinmodule.h
    │   │       ├── boolobject.h
    │   │       ├── bytearrayobject.h
    │   │       ├── bytesobject.h
    │   │       ├── ceval.h
    │   │       ├── codecs.h
    │   │       ├── compile.h
    │   │       ├── complexobject.h
    │   │       ├── cpython
    │   │       │   ├── abstract.h
    │   │       │   ├── bytearrayobject.h
    │   │       │   ├── bytesobject.h
    │   │       │   ├── cellobject.h
    │   │       │   ├── ceval.h
    │   │       │   ├── classobject.h
    │   │       │   ├── code.h
    │   │       │   ├── compile.h
    │   │       │   ├── complexobject.h
    │   │       │   ├── context.h
    │   │       │   ├── descrobject.h
    │   │       │   ├── dictobject.h
    │   │       │   ├── fileobject.h
    │   │       │   ├── fileutils.h
    │   │       │   ├── floatobject.h
    │   │       │   ├── frameobject.h
    │   │       │   ├── funcobject.h
    │   │       │   ├── genobject.h
    │   │       │   ├── import.h
    │   │       │   ├── initconfig.h
    │   │       │   ├── listobject.h
    │   │       │   ├── longintrepr.h
    │   │       │   ├── longobject.h
    │   │       │   ├── methodobject.h
    │   │       │   ├── modsupport.h
    │   │       │   ├── object.h
    │   │       │   ├── objimpl.h
    │   │       │   ├── odictobject.h
    │   │       │   ├── picklebufobject.h
    │   │       │   ├── pthread_stubs.h
    │   │       │   ├── pyctype.h
    │   │       │   ├── pydebug.h
    │   │       │   ├── pyerrors.h
    │   │       │   ├── pyfpe.h
    │   │       │   ├── pyframe.h
    │   │       │   ├── pylifecycle.h
    │   │       │   ├── pymem.h
    │   │       │   ├── pystate.h
    │   │       │   ├── pythonrun.h
    │   │       │   ├── pythread.h
    │   │       │   ├── pytime.h
    │   │       │   ├── setobject.h
    │   │       │   ├── sysmodule.h
    │   │       │   ├── traceback.h
    │   │       │   ├── tupleobject.h
    │   │       │   ├── unicodeobject.h
    │   │       │   ├── warnings.h
    │   │       │   └── weakrefobject.h
    │   │       ├── datetime.h
    │   │       ├── descrobject.h
    │   │       ├── dictobject.h
    │   │       ├── dynamic_annotations.h
    │   │       ├── enumobject.h
    │   │       ├── errcode.h
    │   │       ├── exports.h
    │   │       ├── fileobject.h
    │   │       ├── fileutils.h
    │   │       ├── floatobject.h
    │   │       ├── frameobject.h
    │   │       ├── genericaliasobject.h
    │   │       ├── import.h
    │   │       ├── internal
    │   │       │   ├── pycore_abstract.h
    │   │       │   ├── pycore_accu.h
    │   │       │   ├── pycore_asdl.h
    │   │       │   ├── pycore_ast.h
    │   │       │   ├── pycore_ast_state.h
    │   │       │   ├── pycore_atomic_funcs.h
    │   │       │   ├── pycore_atomic.h
    │   │       │   ├── pycore_bitutils.h
    │   │       │   ├── pycore_blocks_output_buffer.h
    │   │       │   ├── pycore_bytes_methods.h
    │   │       │   ├── pycore_bytesobject.h
    │   │       │   ├── pycore_call.h
    │   │       │   ├── pycore_ceval.h
    │   │       │   ├── pycore_code.h
    │   │       │   ├── pycore_compile.h
    │   │       │   ├── pycore_condvar.h
    │   │       │   ├── pycore_context.h
    │   │       │   ├── pycore_dict.h
    │   │       │   ├── pycore_dtoa.h
    │   │       │   ├── pycore_emscripten_signal.h
    │   │       │   ├── pycore_exceptions.h
    │   │       │   ├── pycore_fileutils.h
    │   │       │   ├── pycore_floatobject.h
    │   │       │   ├── pycore_format.h
    │   │       │   ├── pycore_frame.h
    │   │       │   ├── pycore_function.h
    │   │       │   ├── pycore_gc.h
    │   │       │   ├── pycore_genobject.h
    │   │       │   ├── pycore_getopt.h
    │   │       │   ├── pycore_gil.h
    │   │       │   ├── pycore_global_objects.h
    │   │       │   ├── pycore_global_strings.h
    │   │       │   ├── pycore_hamt.h
    │   │       │   ├── pycore_hashtable.h
    │   │       │   ├── pycore_import.h
    │   │       │   ├── pycore_initconfig.h
    │   │       │   ├── pycore_interp.h
    │   │       │   ├── pycore_interpreteridobject.h
    │   │       │   ├── pycore_list.h
    │   │       │   ├── pycore_long.h
    │   │       │   ├── pycore_moduleobject.h
    │   │       │   ├── pycore_namespace.h
    │   │       │   ├── pycore_object.h
    │   │       │   ├── pycore_opcode.h
    │   │       │   ├── pycore_parser.h
    │   │       │   ├── pycore_pathconfig.h
    │   │       │   ├── pycore_pyarena.h
    │   │       │   ├── pycore_pyerrors.h
    │   │       │   ├── pycore_pyhash.h
    │   │       │   ├── pycore_pylifecycle.h
    │   │       │   ├── pycore_pymath.h
    │   │       │   ├── pycore_pymem.h
    │   │       │   ├── pycore_pystate.h
    │   │       │   ├── pycore_runtime.h
    │   │       │   ├── pycore_runtime_init.h
    │   │       │   ├── pycore_signal.h
    │   │       │   ├── pycore_sliceobject.h
    │   │       │   ├── pycore_strhex.h
    │   │       │   ├── pycore_structseq.h
    │   │       │   ├── pycore_symtable.h
    │   │       │   ├── pycore_sysmodule.h
    │   │       │   ├── pycore_traceback.h
    │   │       │   ├── pycore_tuple.h
    │   │       │   ├── pycore_typeobject.h
    │   │       │   ├── pycore_ucnhash.h
    │   │       │   ├── pycore_unicodeobject.h
    │   │       │   ├── pycore_unionobject.h
    │   │       │   └── pycore_warnings.h
    │   │       ├── intrcheck.h
    │   │       ├── iterobject.h
    │   │       ├── listobject.h
    │   │       ├── longobject.h
    │   │       ├── marshal.h
    │   │       ├── memoryobject.h
    │   │       ├── methodobject.h
    │   │       ├── modsupport.h
    │   │       ├── moduleobject.h
    │   │       ├── object.h
    │   │       ├── objimpl.h
    │   │       ├── opcode.h
    │   │       ├── osdefs.h
    │   │       ├── osmodule.h
    │   │       ├── patchlevel.h
    │   │       ├── pybuffer.h
    │   │       ├── pycapsule.h
    │   │       ├── pyconfig.h
    │   │       ├── py_curses.h
    │   │       ├── pydtrace.h
    │   │       ├── pyerrors.h
    │   │       ├── pyexpat.h
    │   │       ├── pyframe.h
    │   │       ├── pyhash.h
    │   │       ├── pylifecycle.h
    │   │       ├── pymacconfig.h
    │   │       ├── pymacro.h
    │   │       ├── pymath.h
    │   │       ├── pymem.h
    │   │       ├── pyport.h
    │   │       ├── pystate.h
    │   │       ├── pystrcmp.h
    │   │       ├── pystrtod.h
    │   │       ├── Python.h
    │   │       ├── pythonrun.h
    │   │       ├── pythread.h
    │   │       ├── pytypedefs.h
    │   │       ├── rangeobject.h
    │   │       ├── setobject.h
    │   │       ├── sliceobject.h
    │   │       ├── structmember.h
    │   │       ├── structseq.h
    │   │       ├── sysmodule.h
    │   │       ├── token.h
    │   │       ├── traceback.h
    │   │       ├── tracemalloc.h
    │   │       ├── tupleobject.h
    │   │       ├── typeslots.h
    │   │       ├── unicodeobject.h
    │   │       ├── warnings.h
    │   │       └── weakrefobject.h
    │   ├── lib
    │   │   ├── libpython3.11.a
    │   │   ├── pkgconfig
    │   │   │   ├── python-3.11-embed.pc
    │   │   │   ├── python-3.11.pc
    │   │   │   ├── python3-embed.pc -> python-3.11-embed.pc
    │   │   │   └── python3.pc -> python-3.11.pc
    │   │   └── python3.11
    │   │       ├── abc.py
    │   │       ├── aifc.py
    │   │       ├── _aix_support.py
    │   │       ├── antigravity.py
    │   │       ├── argparse.py
    │   │       ├── ast.py
    │   │       ├── asynchat.py
    │   │       ├── asyncio
    │   │       │   ├── base_events.py
    │   │       │   ├── base_futures.py
    │   │       │   ├── base_subprocess.py
    │   │       │   ├── base_tasks.py
    │   │       │   ├── constants.py
    │   │       │   ├── coroutines.py
    │   │       │   ├── events.py
    │   │       │   ├── exceptions.py
    │   │       │   ├── format_helpers.py
    │   │       │   ├── futures.py
    │   │       │   ├── __init__.py
    │   │       │   ├── locks.py
    │   │       │   ├── log.py
    │   │       │   ├── __main__.py
    │   │       │   ├── mixins.py
    │   │       │   ├── proactor_events.py
    │   │       │   ├── protocols.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── base_events.cpython-311.opt-1.pyc
    │   │       │   │   ├── base_events.cpython-311.opt-2.pyc
    │   │       │   │   ├── base_events.cpython-311.pyc
    │   │       │   │   ├── base_futures.cpython-311.opt-1.pyc
    │   │       │   │   ├── base_futures.cpython-311.opt-2.pyc
    │   │       │   │   ├── base_futures.cpython-311.pyc
    │   │       │   │   ├── base_subprocess.cpython-311.opt-1.pyc
    │   │       │   │   ├── base_subprocess.cpython-311.opt-2.pyc
    │   │       │   │   ├── base_subprocess.cpython-311.pyc
    │   │       │   │   ├── base_tasks.cpython-311.opt-1.pyc
    │   │       │   │   ├── base_tasks.cpython-311.opt-2.pyc
    │   │       │   │   ├── base_tasks.cpython-311.pyc
    │   │       │   │   ├── constants.cpython-311.opt-1.pyc
    │   │       │   │   ├── constants.cpython-311.opt-2.pyc
    │   │       │   │   ├── constants.cpython-311.pyc
    │   │       │   │   ├── coroutines.cpython-311.opt-1.pyc
    │   │       │   │   ├── coroutines.cpython-311.opt-2.pyc
    │   │       │   │   ├── coroutines.cpython-311.pyc
    │   │       │   │   ├── events.cpython-311.opt-1.pyc
    │   │       │   │   ├── events.cpython-311.opt-2.pyc
    │   │       │   │   ├── events.cpython-311.pyc
    │   │       │   │   ├── exceptions.cpython-311.opt-1.pyc
    │   │       │   │   ├── exceptions.cpython-311.opt-2.pyc
    │   │       │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │   ├── format_helpers.cpython-311.opt-1.pyc
    │   │       │   │   ├── format_helpers.cpython-311.opt-2.pyc
    │   │       │   │   ├── format_helpers.cpython-311.pyc
    │   │       │   │   ├── futures.cpython-311.opt-1.pyc
    │   │       │   │   ├── futures.cpython-311.opt-2.pyc
    │   │       │   │   ├── futures.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── locks.cpython-311.opt-1.pyc
    │   │       │   │   ├── locks.cpython-311.opt-2.pyc
    │   │       │   │   ├── locks.cpython-311.pyc
    │   │       │   │   ├── log.cpython-311.opt-1.pyc
    │   │       │   │   ├── log.cpython-311.opt-2.pyc
    │   │       │   │   ├── log.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── mixins.cpython-311.opt-1.pyc
    │   │       │   │   ├── mixins.cpython-311.opt-2.pyc
    │   │       │   │   ├── mixins.cpython-311.pyc
    │   │       │   │   ├── proactor_events.cpython-311.opt-1.pyc
    │   │       │   │   ├── proactor_events.cpython-311.opt-2.pyc
    │   │       │   │   ├── proactor_events.cpython-311.pyc
    │   │       │   │   ├── protocols.cpython-311.opt-1.pyc
    │   │       │   │   ├── protocols.cpython-311.opt-2.pyc
    │   │       │   │   ├── protocols.cpython-311.pyc
    │   │       │   │   ├── queues.cpython-311.opt-1.pyc
    │   │       │   │   ├── queues.cpython-311.opt-2.pyc
    │   │       │   │   ├── queues.cpython-311.pyc
    │   │       │   │   ├── runners.cpython-311.opt-1.pyc
    │   │       │   │   ├── runners.cpython-311.opt-2.pyc
    │   │       │   │   ├── runners.cpython-311.pyc
    │   │       │   │   ├── selector_events.cpython-311.opt-1.pyc
    │   │       │   │   ├── selector_events.cpython-311.opt-2.pyc
    │   │       │   │   ├── selector_events.cpython-311.pyc
    │   │       │   │   ├── sslproto.cpython-311.opt-1.pyc
    │   │       │   │   ├── sslproto.cpython-311.opt-2.pyc
    │   │       │   │   ├── sslproto.cpython-311.pyc
    │   │       │   │   ├── staggered.cpython-311.opt-1.pyc
    │   │       │   │   ├── staggered.cpython-311.opt-2.pyc
    │   │       │   │   ├── staggered.cpython-311.pyc
    │   │       │   │   ├── streams.cpython-311.opt-1.pyc
    │   │       │   │   ├── streams.cpython-311.opt-2.pyc
    │   │       │   │   ├── streams.cpython-311.pyc
    │   │       │   │   ├── subprocess.cpython-311.opt-1.pyc
    │   │       │   │   ├── subprocess.cpython-311.opt-2.pyc
    │   │       │   │   ├── subprocess.cpython-311.pyc
    │   │       │   │   ├── taskgroups.cpython-311.opt-1.pyc
    │   │       │   │   ├── taskgroups.cpython-311.opt-2.pyc
    │   │       │   │   ├── taskgroups.cpython-311.pyc
    │   │       │   │   ├── tasks.cpython-311.opt-1.pyc
    │   │       │   │   ├── tasks.cpython-311.opt-2.pyc
    │   │       │   │   ├── tasks.cpython-311.pyc
    │   │       │   │   ├── threads.cpython-311.opt-1.pyc
    │   │       │   │   ├── threads.cpython-311.opt-2.pyc
    │   │       │   │   ├── threads.cpython-311.pyc
    │   │       │   │   ├── timeouts.cpython-311.opt-1.pyc
    │   │       │   │   ├── timeouts.cpython-311.opt-2.pyc
    │   │       │   │   ├── timeouts.cpython-311.pyc
    │   │       │   │   ├── transports.cpython-311.opt-1.pyc
    │   │       │   │   ├── transports.cpython-311.opt-2.pyc
    │   │       │   │   ├── transports.cpython-311.pyc
    │   │       │   │   ├── trsock.cpython-311.opt-1.pyc
    │   │       │   │   ├── trsock.cpython-311.opt-2.pyc
    │   │       │   │   ├── trsock.cpython-311.pyc
    │   │       │   │   ├── unix_events.cpython-311.opt-1.pyc
    │   │       │   │   ├── unix_events.cpython-311.opt-2.pyc
    │   │       │   │   ├── unix_events.cpython-311.pyc
    │   │       │   │   ├── windows_events.cpython-311.opt-1.pyc
    │   │       │   │   ├── windows_events.cpython-311.opt-2.pyc
    │   │       │   │   ├── windows_events.cpython-311.pyc
    │   │       │   │   ├── windows_utils.cpython-311.opt-1.pyc
    │   │       │   │   ├── windows_utils.cpython-311.opt-2.pyc
    │   │       │   │   └── windows_utils.cpython-311.pyc
    │   │       │   ├── queues.py
    │   │       │   ├── runners.py
    │   │       │   ├── selector_events.py
    │   │       │   ├── sslproto.py
    │   │       │   ├── staggered.py
    │   │       │   ├── streams.py
    │   │       │   ├── subprocess.py
    │   │       │   ├── taskgroups.py
    │   │       │   ├── tasks.py
    │   │       │   ├── threads.py
    │   │       │   ├── timeouts.py
    │   │       │   ├── transports.py
    │   │       │   ├── trsock.py
    │   │       │   ├── unix_events.py
    │   │       │   ├── windows_events.py
    │   │       │   └── windows_utils.py
    │   │       ├── asyncore.py
    │   │       ├── base64.py
    │   │       ├── bdb.py
    │   │       ├── bisect.py
    │   │       ├── _bootsubprocess.py
    │   │       ├── bz2.py
    │   │       ├── calendar.py
    │   │       ├── cgi.py
    │   │       ├── cgitb.py
    │   │       ├── chunk.py
    │   │       ├── cmd.py
    │   │       ├── codecs.py
    │   │       ├── codeop.py
    │   │       ├── code.py
    │   │       ├── collections
    │   │       │   ├── abc.py
    │   │       │   ├── __init__.py
    │   │       │   └── __pycache__
    │   │       │       ├── abc.cpython-311.opt-1.pyc
    │   │       │       ├── abc.cpython-311.opt-2.pyc
    │   │       │       ├── abc.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       └── __init__.cpython-311.pyc
    │   │       ├── _collections_abc.py
    │   │       ├── colorsys.py
    │   │       ├── _compat_pickle.py
    │   │       ├── compileall.py
    │   │       ├── _compression.py
    │   │       ├── concurrent
    │   │       │   ├── futures
    │   │       │   │   ├── _base.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── process.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── _base.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _base.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _base.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── process.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── process.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── process.cpython-311.pyc
    │   │       │   │   │   ├── thread.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── thread.cpython-311.opt-2.pyc
    │   │       │   │   │   └── thread.cpython-311.pyc
    │   │       │   │   └── thread.py
    │   │       │   ├── __init__.py
    │   │       │   └── __pycache__
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       └── __init__.cpython-311.pyc
    │   │       ├── config-3.11-x86_64-linux-gnu
    │   │       │   ├── config.c
    │   │       │   ├── config.c.in
    │   │       │   ├── install-sh
    │   │       │   ├── libpython3.11.a
    │   │       │   ├── Makefile
    │   │       │   ├── makesetup
    │   │       │   ├── __pycache__
    │   │       │   │   ├── python-config.cpython-311.opt-1.pyc
    │   │       │   │   ├── python-config.cpython-311.opt-2.pyc
    │   │       │   │   └── python-config.cpython-311.pyc
    │   │       │   ├── python-config.py
    │   │       │   ├── python.o
    │   │       │   ├── Setup
    │   │       │   ├── Setup.bootstrap
    │   │       │   ├── Setup.local
    │   │       │   └── Setup.stdlib
    │   │       ├── configparser.py
    │   │       ├── contextlib.py
    │   │       ├── contextvars.py
    │   │       ├── copy.py
    │   │       ├── copyreg.py
    │   │       ├── cProfile.py
    │   │       ├── crypt.py
    │   │       ├── csv.py
    │   │       ├── ctypes
    │   │       │   ├── _aix.py
    │   │       │   ├── _endian.py
    │   │       │   ├── __init__.py
    │   │       │   ├── macholib
    │   │       │   │   ├── dyld.py
    │   │       │   │   ├── dylib.py
    │   │       │   │   ├── fetch_macholib
    │   │       │   │   ├── fetch_macholib.bat
    │   │       │   │   ├── framework.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── dyld.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── dyld.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── dyld.cpython-311.pyc
    │   │       │   │   │   ├── dylib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── dylib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── dylib.cpython-311.pyc
    │   │       │   │   │   ├── framework.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── framework.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── framework.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   └── README.ctypes
    │   │       │   ├── __pycache__
    │   │       │   │   ├── _aix.cpython-311.opt-1.pyc
    │   │       │   │   ├── _aix.cpython-311.opt-2.pyc
    │   │       │   │   ├── _aix.cpython-311.pyc
    │   │       │   │   ├── _endian.cpython-311.opt-1.pyc
    │   │       │   │   ├── _endian.cpython-311.opt-2.pyc
    │   │       │   │   ├── _endian.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   ├── util.cpython-311.pyc
    │   │       │   │   ├── wintypes.cpython-311.opt-1.pyc
    │   │       │   │   ├── wintypes.cpython-311.opt-2.pyc
    │   │       │   │   └── wintypes.cpython-311.pyc
    │   │       │   ├── test
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_anon.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_anon.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_anon.cpython-311.pyc
    │   │       │   │   │   ├── test_array_in_pointer.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_array_in_pointer.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_array_in_pointer.cpython-311.pyc
    │   │       │   │   │   ├── test_arrays.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_arrays.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_arrays.cpython-311.pyc
    │   │       │   │   │   ├── test_as_parameter.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_as_parameter.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_as_parameter.cpython-311.pyc
    │   │       │   │   │   ├── test_bitfields.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_bitfields.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_bitfields.cpython-311.pyc
    │   │       │   │   │   ├── test_buffers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_buffers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_buffers.cpython-311.pyc
    │   │       │   │   │   ├── test_bytes.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_bytes.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_bytes.cpython-311.pyc
    │   │       │   │   │   ├── test_byteswap.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_byteswap.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_byteswap.cpython-311.pyc
    │   │       │   │   │   ├── test_callbacks.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_callbacks.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_callbacks.cpython-311.pyc
    │   │       │   │   │   ├── test_cast.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_cast.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_cast.cpython-311.pyc
    │   │       │   │   │   ├── test_cfuncs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_cfuncs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_cfuncs.cpython-311.pyc
    │   │       │   │   │   ├── test_checkretval.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_checkretval.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_checkretval.cpython-311.pyc
    │   │       │   │   │   ├── test_delattr.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_delattr.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_delattr.cpython-311.pyc
    │   │       │   │   │   ├── test_errno.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_errno.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_errno.cpython-311.pyc
    │   │       │   │   │   ├── test_find.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_find.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_find.cpython-311.pyc
    │   │       │   │   │   ├── test_frombuffer.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_frombuffer.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_frombuffer.cpython-311.pyc
    │   │       │   │   │   ├── test_funcptr.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_funcptr.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_funcptr.cpython-311.pyc
    │   │       │   │   │   ├── test_functions.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_functions.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_functions.cpython-311.pyc
    │   │       │   │   │   ├── test_incomplete.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_incomplete.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_incomplete.cpython-311.pyc
    │   │       │   │   │   ├── test_init.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_init.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_init.cpython-311.pyc
    │   │       │   │   │   ├── test_internals.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_internals.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_internals.cpython-311.pyc
    │   │       │   │   │   ├── test_keeprefs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_keeprefs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_keeprefs.cpython-311.pyc
    │   │       │   │   │   ├── test_libc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_libc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_libc.cpython-311.pyc
    │   │       │   │   │   ├── test_loading.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_loading.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_loading.cpython-311.pyc
    │   │       │   │   │   ├── test_macholib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_macholib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_macholib.cpython-311.pyc
    │   │       │   │   │   ├── test_memfunctions.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_memfunctions.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_memfunctions.cpython-311.pyc
    │   │       │   │   │   ├── test_numbers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_numbers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_numbers.cpython-311.pyc
    │   │       │   │   │   ├── test_objects.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_objects.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_objects.cpython-311.pyc
    │   │       │   │   │   ├── test_parameters.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_parameters.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_parameters.cpython-311.pyc
    │   │       │   │   │   ├── test_pep3118.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pep3118.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pep3118.cpython-311.pyc
    │   │       │   │   │   ├── test_pickling.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pickling.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pickling.cpython-311.pyc
    │   │       │   │   │   ├── test_pointers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pointers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pointers.cpython-311.pyc
    │   │       │   │   │   ├── test_prototypes.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_prototypes.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_prototypes.cpython-311.pyc
    │   │       │   │   │   ├── test_python_api.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_python_api.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_python_api.cpython-311.pyc
    │   │       │   │   │   ├── test_random_things.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_random_things.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_random_things.cpython-311.pyc
    │   │       │   │   │   ├── test_refcounts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_refcounts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_refcounts.cpython-311.pyc
    │   │       │   │   │   ├── test_repr.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_repr.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_repr.cpython-311.pyc
    │   │       │   │   │   ├── test_returnfuncptrs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_returnfuncptrs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_returnfuncptrs.cpython-311.pyc
    │   │       │   │   │   ├── test_simplesubclasses.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_simplesubclasses.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_simplesubclasses.cpython-311.pyc
    │   │       │   │   │   ├── test_sizes.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sizes.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sizes.cpython-311.pyc
    │   │       │   │   │   ├── test_slicing.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_slicing.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_slicing.cpython-311.pyc
    │   │       │   │   │   ├── test_stringptr.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_stringptr.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_stringptr.cpython-311.pyc
    │   │       │   │   │   ├── test_strings.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_strings.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_strings.cpython-311.pyc
    │   │       │   │   │   ├── test_struct_fields.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_struct_fields.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_struct_fields.cpython-311.pyc
    │   │       │   │   │   ├── test_structures.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_structures.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_structures.cpython-311.pyc
    │   │       │   │   │   ├── test_unaligned_structures.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unaligned_structures.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_unaligned_structures.cpython-311.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.pyc
    │   │       │   │   │   ├── test_values.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_values.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_values.cpython-311.pyc
    │   │       │   │   │   ├── test_varsize_struct.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_varsize_struct.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_varsize_struct.cpython-311.pyc
    │   │       │   │   │   ├── test_win32.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_win32.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_win32.cpython-311.pyc
    │   │       │   │   │   ├── test_wintypes.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_wintypes.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_wintypes.cpython-311.pyc
    │   │       │   │   ├── test_anon.py
    │   │       │   │   ├── test_array_in_pointer.py
    │   │       │   │   ├── test_arrays.py
    │   │       │   │   ├── test_as_parameter.py
    │   │       │   │   ├── test_bitfields.py
    │   │       │   │   ├── test_buffers.py
    │   │       │   │   ├── test_bytes.py
    │   │       │   │   ├── test_byteswap.py
    │   │       │   │   ├── test_callbacks.py
    │   │       │   │   ├── test_cast.py
    │   │       │   │   ├── test_cfuncs.py
    │   │       │   │   ├── test_checkretval.py
    │   │       │   │   ├── test_delattr.py
    │   │       │   │   ├── test_errno.py
    │   │       │   │   ├── test_find.py
    │   │       │   │   ├── test_frombuffer.py
    │   │       │   │   ├── test_funcptr.py
    │   │       │   │   ├── test_functions.py
    │   │       │   │   ├── test_incomplete.py
    │   │       │   │   ├── test_init.py
    │   │       │   │   ├── test_internals.py
    │   │       │   │   ├── test_keeprefs.py
    │   │       │   │   ├── test_libc.py
    │   │       │   │   ├── test_loading.py
    │   │       │   │   ├── test_macholib.py
    │   │       │   │   ├── test_memfunctions.py
    │   │       │   │   ├── test_numbers.py
    │   │       │   │   ├── test_objects.py
    │   │       │   │   ├── test_parameters.py
    │   │       │   │   ├── test_pep3118.py
    │   │       │   │   ├── test_pickling.py
    │   │       │   │   ├── test_pointers.py
    │   │       │   │   ├── test_prototypes.py
    │   │       │   │   ├── test_python_api.py
    │   │       │   │   ├── test_random_things.py
    │   │       │   │   ├── test_refcounts.py
    │   │       │   │   ├── test_repr.py
    │   │       │   │   ├── test_returnfuncptrs.py
    │   │       │   │   ├── test_simplesubclasses.py
    │   │       │   │   ├── test_sizes.py
    │   │       │   │   ├── test_slicing.py
    │   │       │   │   ├── test_stringptr.py
    │   │       │   │   ├── test_strings.py
    │   │       │   │   ├── test_struct_fields.py
    │   │       │   │   ├── test_structures.py
    │   │       │   │   ├── test_unaligned_structures.py
    │   │       │   │   ├── test_unicode.py
    │   │       │   │   ├── test_values.py
    │   │       │   │   ├── test_varsize_struct.py
    │   │       │   │   ├── test_win32.py
    │   │       │   │   └── test_wintypes.py
    │   │       │   ├── util.py
    │   │       │   └── wintypes.py
    │   │       ├── curses
    │   │       │   ├── ascii.py
    │   │       │   ├── has_key.py
    │   │       │   ├── __init__.py
    │   │       │   ├── panel.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── ascii.cpython-311.opt-1.pyc
    │   │       │   │   ├── ascii.cpython-311.opt-2.pyc
    │   │       │   │   ├── ascii.cpython-311.pyc
    │   │       │   │   ├── has_key.cpython-311.opt-1.pyc
    │   │       │   │   ├── has_key.cpython-311.opt-2.pyc
    │   │       │   │   ├── has_key.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── panel.cpython-311.opt-1.pyc
    │   │       │   │   ├── panel.cpython-311.opt-2.pyc
    │   │       │   │   ├── panel.cpython-311.pyc
    │   │       │   │   ├── textpad.cpython-311.opt-1.pyc
    │   │       │   │   ├── textpad.cpython-311.opt-2.pyc
    │   │       │   │   └── textpad.cpython-311.pyc
    │   │       │   └── textpad.py
    │   │       ├── dataclasses.py
    │   │       ├── datetime.py
    │   │       ├── dbm
    │   │       │   ├── dumb.py
    │   │       │   ├── gnu.py
    │   │       │   ├── __init__.py
    │   │       │   ├── ndbm.py
    │   │       │   └── __pycache__
    │   │       │       ├── dumb.cpython-311.opt-1.pyc
    │   │       │       ├── dumb.cpython-311.opt-2.pyc
    │   │       │       ├── dumb.cpython-311.pyc
    │   │       │       ├── gnu.cpython-311.opt-1.pyc
    │   │       │       ├── gnu.cpython-311.opt-2.pyc
    │   │       │       ├── gnu.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       ├── __init__.cpython-311.pyc
    │   │       │       ├── ndbm.cpython-311.opt-1.pyc
    │   │       │       ├── ndbm.cpython-311.opt-2.pyc
    │   │       │       └── ndbm.cpython-311.pyc
    │   │       ├── decimal.py
    │   │       ├── difflib.py
    │   │       ├── dis.py
    │   │       ├── distutils
    │   │       │   ├── archive_util.py
    │   │       │   ├── bcppcompiler.py
    │   │       │   ├── ccompiler.py
    │   │       │   ├── cmd.py
    │   │       │   ├── command
    │   │       │   │   ├── bdist_dumb.py
    │   │       │   │   ├── bdist.py
    │   │       │   │   ├── bdist_rpm.py
    │   │       │   │   ├── build_clib.py
    │   │       │   │   ├── build_ext.py
    │   │       │   │   ├── build.py
    │   │       │   │   ├── build_py.py
    │   │       │   │   ├── build_scripts.py
    │   │       │   │   ├── check.py
    │   │       │   │   ├── clean.py
    │   │       │   │   ├── command_template
    │   │       │   │   ├── config.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── install_data.py
    │   │       │   │   ├── install_egg_info.py
    │   │       │   │   ├── install_headers.py
    │   │       │   │   ├── install_lib.py
    │   │       │   │   ├── install.py
    │   │       │   │   ├── install_scripts.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── bdist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── bdist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── bdist.cpython-311.pyc
    │   │       │   │   │   ├── bdist_dumb.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── bdist_dumb.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── bdist_dumb.cpython-311.pyc
    │   │       │   │   │   ├── bdist_rpm.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── bdist_rpm.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── bdist_rpm.cpython-311.pyc
    │   │       │   │   │   ├── build_clib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── build_clib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── build_clib.cpython-311.pyc
    │   │       │   │   │   ├── build.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── build.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── build.cpython-311.pyc
    │   │       │   │   │   ├── build_ext.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── build_ext.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── build_ext.cpython-311.pyc
    │   │       │   │   │   ├── build_py.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── build_py.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── build_py.cpython-311.pyc
    │   │       │   │   │   ├── build_scripts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── build_scripts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── build_scripts.cpython-311.pyc
    │   │       │   │   │   ├── check.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── check.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── check.cpython-311.pyc
    │   │       │   │   │   ├── clean.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── clean.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── clean.cpython-311.pyc
    │   │       │   │   │   ├── config.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── config.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── config.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── install.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install.cpython-311.pyc
    │   │       │   │   │   ├── install_data.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install_data.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install_data.cpython-311.pyc
    │   │       │   │   │   ├── install_egg_info.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install_egg_info.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install_egg_info.cpython-311.pyc
    │   │       │   │   │   ├── install_headers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install_headers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install_headers.cpython-311.pyc
    │   │       │   │   │   ├── install_lib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install_lib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install_lib.cpython-311.pyc
    │   │       │   │   │   ├── install_scripts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── install_scripts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── install_scripts.cpython-311.pyc
    │   │       │   │   │   ├── register.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── register.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── register.cpython-311.pyc
    │   │       │   │   │   ├── sdist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── sdist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── sdist.cpython-311.pyc
    │   │       │   │   │   ├── upload.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── upload.cpython-311.opt-2.pyc
    │   │       │   │   │   └── upload.cpython-311.pyc
    │   │       │   │   ├── register.py
    │   │       │   │   ├── sdist.py
    │   │       │   │   └── upload.py
    │   │       │   ├── config.py
    │   │       │   ├── core.py
    │   │       │   ├── cygwinccompiler.py
    │   │       │   ├── debug.py
    │   │       │   ├── dep_util.py
    │   │       │   ├── dir_util.py
    │   │       │   ├── dist.py
    │   │       │   ├── errors.py
    │   │       │   ├── extension.py
    │   │       │   ├── fancy_getopt.py
    │   │       │   ├── filelist.py
    │   │       │   ├── file_util.py
    │   │       │   ├── __init__.py
    │   │       │   ├── log.py
    │   │       │   ├── msvc9compiler.py
    │   │       │   ├── _msvccompiler.py
    │   │       │   ├── msvccompiler.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── archive_util.cpython-311.opt-1.pyc
    │   │       │   │   ├── archive_util.cpython-311.opt-2.pyc
    │   │       │   │   ├── archive_util.cpython-311.pyc
    │   │       │   │   ├── bcppcompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── bcppcompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── bcppcompiler.cpython-311.pyc
    │   │       │   │   ├── ccompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── ccompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── ccompiler.cpython-311.pyc
    │   │       │   │   ├── cmd.cpython-311.opt-1.pyc
    │   │       │   │   ├── cmd.cpython-311.opt-2.pyc
    │   │       │   │   ├── cmd.cpython-311.pyc
    │   │       │   │   ├── config.cpython-311.opt-1.pyc
    │   │       │   │   ├── config.cpython-311.opt-2.pyc
    │   │       │   │   ├── config.cpython-311.pyc
    │   │       │   │   ├── core.cpython-311.opt-1.pyc
    │   │       │   │   ├── core.cpython-311.opt-2.pyc
    │   │       │   │   ├── core.cpython-311.pyc
    │   │       │   │   ├── cygwinccompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── cygwinccompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── cygwinccompiler.cpython-311.pyc
    │   │       │   │   ├── debug.cpython-311.opt-1.pyc
    │   │       │   │   ├── debug.cpython-311.opt-2.pyc
    │   │       │   │   ├── debug.cpython-311.pyc
    │   │       │   │   ├── dep_util.cpython-311.opt-1.pyc
    │   │       │   │   ├── dep_util.cpython-311.opt-2.pyc
    │   │       │   │   ├── dep_util.cpython-311.pyc
    │   │       │   │   ├── dir_util.cpython-311.opt-1.pyc
    │   │       │   │   ├── dir_util.cpython-311.opt-2.pyc
    │   │       │   │   ├── dir_util.cpython-311.pyc
    │   │       │   │   ├── dist.cpython-311.opt-1.pyc
    │   │       │   │   ├── dist.cpython-311.opt-2.pyc
    │   │       │   │   ├── dist.cpython-311.pyc
    │   │       │   │   ├── errors.cpython-311.opt-1.pyc
    │   │       │   │   ├── errors.cpython-311.opt-2.pyc
    │   │       │   │   ├── errors.cpython-311.pyc
    │   │       │   │   ├── extension.cpython-311.opt-1.pyc
    │   │       │   │   ├── extension.cpython-311.opt-2.pyc
    │   │       │   │   ├── extension.cpython-311.pyc
    │   │       │   │   ├── fancy_getopt.cpython-311.opt-1.pyc
    │   │       │   │   ├── fancy_getopt.cpython-311.opt-2.pyc
    │   │       │   │   ├── fancy_getopt.cpython-311.pyc
    │   │       │   │   ├── filelist.cpython-311.opt-1.pyc
    │   │       │   │   ├── filelist.cpython-311.opt-2.pyc
    │   │       │   │   ├── filelist.cpython-311.pyc
    │   │       │   │   ├── file_util.cpython-311.opt-1.pyc
    │   │       │   │   ├── file_util.cpython-311.opt-2.pyc
    │   │       │   │   ├── file_util.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── log.cpython-311.opt-1.pyc
    │   │       │   │   ├── log.cpython-311.opt-2.pyc
    │   │       │   │   ├── log.cpython-311.pyc
    │   │       │   │   ├── msvc9compiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── msvc9compiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── msvc9compiler.cpython-311.pyc
    │   │       │   │   ├── _msvccompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── msvccompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── _msvccompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── msvccompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── _msvccompiler.cpython-311.pyc
    │   │       │   │   ├── msvccompiler.cpython-311.pyc
    │   │       │   │   ├── spawn.cpython-311.opt-1.pyc
    │   │       │   │   ├── spawn.cpython-311.opt-2.pyc
    │   │       │   │   ├── spawn.cpython-311.pyc
    │   │       │   │   ├── sysconfig.cpython-311.opt-1.pyc
    │   │       │   │   ├── sysconfig.cpython-311.opt-2.pyc
    │   │       │   │   ├── sysconfig.cpython-311.pyc
    │   │       │   │   ├── text_file.cpython-311.opt-1.pyc
    │   │       │   │   ├── text_file.cpython-311.opt-2.pyc
    │   │       │   │   ├── text_file.cpython-311.pyc
    │   │       │   │   ├── unixccompiler.cpython-311.opt-1.pyc
    │   │       │   │   ├── unixccompiler.cpython-311.opt-2.pyc
    │   │       │   │   ├── unixccompiler.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   ├── util.cpython-311.pyc
    │   │       │   │   ├── version.cpython-311.opt-1.pyc
    │   │       │   │   ├── version.cpython-311.opt-2.pyc
    │   │       │   │   ├── version.cpython-311.pyc
    │   │       │   │   ├── versionpredicate.cpython-311.opt-1.pyc
    │   │       │   │   ├── versionpredicate.cpython-311.opt-2.pyc
    │   │       │   │   └── versionpredicate.cpython-311.pyc
    │   │       │   ├── README
    │   │       │   ├── spawn.py
    │   │       │   ├── sysconfig.py
    │   │       │   ├── tests
    │   │       │   │   ├── includetest.rst
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── support.cpython-311.pyc
    │   │       │   │   │   ├── test_archive_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_archive_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_archive_util.cpython-311.pyc
    │   │       │   │   │   ├── test_bdist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_bdist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_bdist.cpython-311.pyc
    │   │       │   │   │   ├── test_bdist_dumb.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_bdist_dumb.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_bdist_dumb.cpython-311.pyc
    │   │       │   │   │   ├── test_bdist_rpm.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_bdist_rpm.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_bdist_rpm.cpython-311.pyc
    │   │       │   │   │   ├── test_build_clib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_build_clib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_build_clib.cpython-311.pyc
    │   │       │   │   │   ├── test_build.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_build.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_build.cpython-311.pyc
    │   │       │   │   │   ├── test_build_ext.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_build_ext.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_build_ext.cpython-311.pyc
    │   │       │   │   │   ├── test_build_py.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_build_py.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_build_py.cpython-311.pyc
    │   │       │   │   │   ├── test_build_scripts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_build_scripts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_build_scripts.cpython-311.pyc
    │   │       │   │   │   ├── test_check.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_check.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_check.cpython-311.pyc
    │   │       │   │   │   ├── test_clean.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_clean.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_clean.cpython-311.pyc
    │   │       │   │   │   ├── test_cmd.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_cmd.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_cmd.cpython-311.pyc
    │   │       │   │   │   ├── test_config_cmd.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_config_cmd.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_config_cmd.cpython-311.pyc
    │   │       │   │   │   ├── test_config.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_config.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_config.cpython-311.pyc
    │   │       │   │   │   ├── test_core.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_core.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_core.cpython-311.pyc
    │   │       │   │   │   ├── test_cygwinccompiler.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_cygwinccompiler.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_cygwinccompiler.cpython-311.pyc
    │   │       │   │   │   ├── test_dep_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dep_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dep_util.cpython-311.pyc
    │   │       │   │   │   ├── test_dir_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dir_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dir_util.cpython-311.pyc
    │   │       │   │   │   ├── test_dist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dist.cpython-311.pyc
    │   │       │   │   │   ├── test_extension.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_extension.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_extension.cpython-311.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.pyc
    │   │       │   │   │   ├── test_file_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_file_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_file_util.cpython-311.pyc
    │   │       │   │   │   ├── test_install.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_install.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_install.cpython-311.pyc
    │   │       │   │   │   ├── test_install_data.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_install_data.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_install_data.cpython-311.pyc
    │   │       │   │   │   ├── test_install_headers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_install_headers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_install_headers.cpython-311.pyc
    │   │       │   │   │   ├── test_install_lib.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_install_lib.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_install_lib.cpython-311.pyc
    │   │       │   │   │   ├── test_install_scripts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_install_scripts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_install_scripts.cpython-311.pyc
    │   │       │   │   │   ├── test_log.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_log.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_log.cpython-311.pyc
    │   │       │   │   │   ├── test_msvc9compiler.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_msvc9compiler.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_msvc9compiler.cpython-311.pyc
    │   │       │   │   │   ├── test_msvccompiler.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_msvccompiler.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_msvccompiler.cpython-311.pyc
    │   │       │   │   │   ├── test_register.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_register.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_register.cpython-311.pyc
    │   │       │   │   │   ├── test_sdist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sdist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sdist.cpython-311.pyc
    │   │       │   │   │   ├── test_spawn.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_spawn.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_spawn.cpython-311.pyc
    │   │       │   │   │   ├── test_sysconfig.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sysconfig.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sysconfig.cpython-311.pyc
    │   │       │   │   │   ├── test_text_file.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_text_file.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_text_file.cpython-311.pyc
    │   │       │   │   │   ├── test_unixccompiler.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unixccompiler.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_unixccompiler.cpython-311.pyc
    │   │       │   │   │   ├── test_upload.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_upload.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_upload.cpython-311.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_util.cpython-311.pyc
    │   │       │   │   │   ├── test_version.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_version.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_version.cpython-311.pyc
    │   │       │   │   │   ├── test_versionpredicate.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_versionpredicate.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_versionpredicate.cpython-311.pyc
    │   │       │   │   ├── Setup.sample
    │   │       │   │   ├── support.py
    │   │       │   │   ├── test_archive_util.py
    │   │       │   │   ├── test_bdist_dumb.py
    │   │       │   │   ├── test_bdist.py
    │   │       │   │   ├── test_bdist_rpm.py
    │   │       │   │   ├── test_build_clib.py
    │   │       │   │   ├── test_build_ext.py
    │   │       │   │   ├── test_build.py
    │   │       │   │   ├── test_build_py.py
    │   │       │   │   ├── test_build_scripts.py
    │   │       │   │   ├── test_check.py
    │   │       │   │   ├── test_clean.py
    │   │       │   │   ├── test_cmd.py
    │   │       │   │   ├── test_config_cmd.py
    │   │       │   │   ├── test_config.py
    │   │       │   │   ├── test_core.py
    │   │       │   │   ├── test_cygwinccompiler.py
    │   │       │   │   ├── test_dep_util.py
    │   │       │   │   ├── test_dir_util.py
    │   │       │   │   ├── test_dist.py
    │   │       │   │   ├── test_extension.py
    │   │       │   │   ├── test_filelist.py
    │   │       │   │   ├── test_file_util.py
    │   │       │   │   ├── test_install_data.py
    │   │       │   │   ├── test_install_headers.py
    │   │       │   │   ├── test_install_lib.py
    │   │       │   │   ├── test_install.py
    │   │       │   │   ├── test_install_scripts.py
    │   │       │   │   ├── test_log.py
    │   │       │   │   ├── test_msvc9compiler.py
    │   │       │   │   ├── test_msvccompiler.py
    │   │       │   │   ├── test_register.py
    │   │       │   │   ├── test_sdist.py
    │   │       │   │   ├── test_spawn.py
    │   │       │   │   ├── test_sysconfig.py
    │   │       │   │   ├── test_text_file.py
    │   │       │   │   ├── test_unixccompiler.py
    │   │       │   │   ├── test_upload.py
    │   │       │   │   ├── test_util.py
    │   │       │   │   ├── test_versionpredicate.py
    │   │       │   │   ├── test_version.py
    │   │       │   │   └── xxmodule.c
    │   │       │   ├── text_file.py
    │   │       │   ├── unixccompiler.py
    │   │       │   ├── util.py
    │   │       │   ├── versionpredicate.py
    │   │       │   └── version.py
    │   │       ├── doctest.py
    │   │       ├── email
    │   │       │   ├── architecture.rst
    │   │       │   ├── base64mime.py
    │   │       │   ├── charset.py
    │   │       │   ├── contentmanager.py
    │   │       │   ├── _encoded_words.py
    │   │       │   ├── encoders.py
    │   │       │   ├── errors.py
    │   │       │   ├── feedparser.py
    │   │       │   ├── generator.py
    │   │       │   ├── header.py
    │   │       │   ├── headerregistry.py
    │   │       │   ├── _header_value_parser.py
    │   │       │   ├── __init__.py
    │   │       │   ├── iterators.py
    │   │       │   ├── message.py
    │   │       │   ├── mime
    │   │       │   │   ├── application.py
    │   │       │   │   ├── audio.py
    │   │       │   │   ├── base.py
    │   │       │   │   ├── image.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── message.py
    │   │       │   │   ├── multipart.py
    │   │       │   │   ├── nonmultipart.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── application.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── application.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── application.cpython-311.pyc
    │   │       │   │   │   ├── audio.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── audio.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── audio.cpython-311.pyc
    │   │       │   │   │   ├── base.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── base.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── base.cpython-311.pyc
    │   │       │   │   │   ├── image.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── image.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── image.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── message.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── message.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── message.cpython-311.pyc
    │   │       │   │   │   ├── multipart.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── multipart.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── multipart.cpython-311.pyc
    │   │       │   │   │   ├── nonmultipart.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── nonmultipart.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── nonmultipart.cpython-311.pyc
    │   │       │   │   │   ├── text.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── text.cpython-311.opt-2.pyc
    │   │       │   │   │   └── text.cpython-311.pyc
    │   │       │   │   └── text.py
    │   │       │   ├── _parseaddr.py
    │   │       │   ├── parser.py
    │   │       │   ├── _policybase.py
    │   │       │   ├── policy.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── base64mime.cpython-311.opt-1.pyc
    │   │       │   │   ├── base64mime.cpython-311.opt-2.pyc
    │   │       │   │   ├── base64mime.cpython-311.pyc
    │   │       │   │   ├── charset.cpython-311.opt-1.pyc
    │   │       │   │   ├── charset.cpython-311.opt-2.pyc
    │   │       │   │   ├── charset.cpython-311.pyc
    │   │       │   │   ├── contentmanager.cpython-311.opt-1.pyc
    │   │       │   │   ├── contentmanager.cpython-311.opt-2.pyc
    │   │       │   │   ├── contentmanager.cpython-311.pyc
    │   │       │   │   ├── _encoded_words.cpython-311.opt-1.pyc
    │   │       │   │   ├── _encoded_words.cpython-311.opt-2.pyc
    │   │       │   │   ├── _encoded_words.cpython-311.pyc
    │   │       │   │   ├── encoders.cpython-311.opt-1.pyc
    │   │       │   │   ├── encoders.cpython-311.opt-2.pyc
    │   │       │   │   ├── encoders.cpython-311.pyc
    │   │       │   │   ├── errors.cpython-311.opt-1.pyc
    │   │       │   │   ├── errors.cpython-311.opt-2.pyc
    │   │       │   │   ├── errors.cpython-311.pyc
    │   │       │   │   ├── feedparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── feedparser.cpython-311.opt-2.pyc
    │   │       │   │   ├── feedparser.cpython-311.pyc
    │   │       │   │   ├── generator.cpython-311.opt-1.pyc
    │   │       │   │   ├── generator.cpython-311.opt-2.pyc
    │   │       │   │   ├── generator.cpython-311.pyc
    │   │       │   │   ├── header.cpython-311.opt-1.pyc
    │   │       │   │   ├── header.cpython-311.opt-2.pyc
    │   │       │   │   ├── header.cpython-311.pyc
    │   │       │   │   ├── headerregistry.cpython-311.opt-1.pyc
    │   │       │   │   ├── headerregistry.cpython-311.opt-2.pyc
    │   │       │   │   ├── headerregistry.cpython-311.pyc
    │   │       │   │   ├── _header_value_parser.cpython-311.opt-1.pyc
    │   │       │   │   ├── _header_value_parser.cpython-311.opt-2.pyc
    │   │       │   │   ├── _header_value_parser.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── iterators.cpython-311.opt-1.pyc
    │   │       │   │   ├── iterators.cpython-311.opt-2.pyc
    │   │       │   │   ├── iterators.cpython-311.pyc
    │   │       │   │   ├── message.cpython-311.opt-1.pyc
    │   │       │   │   ├── message.cpython-311.opt-2.pyc
    │   │       │   │   ├── message.cpython-311.pyc
    │   │       │   │   ├── _parseaddr.cpython-311.opt-1.pyc
    │   │       │   │   ├── _parseaddr.cpython-311.opt-2.pyc
    │   │       │   │   ├── _parseaddr.cpython-311.pyc
    │   │       │   │   ├── parser.cpython-311.opt-1.pyc
    │   │       │   │   ├── parser.cpython-311.opt-2.pyc
    │   │       │   │   ├── parser.cpython-311.pyc
    │   │       │   │   ├── _policybase.cpython-311.opt-1.pyc
    │   │       │   │   ├── _policybase.cpython-311.opt-2.pyc
    │   │       │   │   ├── _policybase.cpython-311.pyc
    │   │       │   │   ├── policy.cpython-311.opt-1.pyc
    │   │       │   │   ├── policy.cpython-311.opt-2.pyc
    │   │       │   │   ├── policy.cpython-311.pyc
    │   │       │   │   ├── quoprimime.cpython-311.opt-1.pyc
    │   │       │   │   ├── quoprimime.cpython-311.opt-2.pyc
    │   │       │   │   ├── quoprimime.cpython-311.pyc
    │   │       │   │   ├── utils.cpython-311.opt-1.pyc
    │   │       │   │   ├── utils.cpython-311.opt-2.pyc
    │   │       │   │   └── utils.cpython-311.pyc
    │   │       │   ├── quoprimime.py
    │   │       │   └── utils.py
    │   │       ├── encodings
    │   │       │   ├── aliases.py
    │   │       │   ├── ascii.py
    │   │       │   ├── base64_codec.py
    │   │       │   ├── big5hkscs.py
    │   │       │   ├── big5.py
    │   │       │   ├── bz2_codec.py
    │   │       │   ├── charmap.py
    │   │       │   ├── cp037.py
    │   │       │   ├── cp1006.py
    │   │       │   ├── cp1026.py
    │   │       │   ├── cp1125.py
    │   │       │   ├── cp1140.py
    │   │       │   ├── cp1250.py
    │   │       │   ├── cp1251.py
    │   │       │   ├── cp1252.py
    │   │       │   ├── cp1253.py
    │   │       │   ├── cp1254.py
    │   │       │   ├── cp1255.py
    │   │       │   ├── cp1256.py
    │   │       │   ├── cp1257.py
    │   │       │   ├── cp1258.py
    │   │       │   ├── cp273.py
    │   │       │   ├── cp424.py
    │   │       │   ├── cp437.py
    │   │       │   ├── cp500.py
    │   │       │   ├── cp720.py
    │   │       │   ├── cp737.py
    │   │       │   ├── cp775.py
    │   │       │   ├── cp850.py
    │   │       │   ├── cp852.py
    │   │       │   ├── cp855.py
    │   │       │   ├── cp856.py
    │   │       │   ├── cp857.py
    │   │       │   ├── cp858.py
    │   │       │   ├── cp860.py
    │   │       │   ├── cp861.py
    │   │       │   ├── cp862.py
    │   │       │   ├── cp863.py
    │   │       │   ├── cp864.py
    │   │       │   ├── cp865.py
    │   │       │   ├── cp866.py
    │   │       │   ├── cp869.py
    │   │       │   ├── cp874.py
    │   │       │   ├── cp875.py
    │   │       │   ├── cp932.py
    │   │       │   ├── cp949.py
    │   │       │   ├── cp950.py
    │   │       │   ├── euc_jis_2004.py
    │   │       │   ├── euc_jisx0213.py
    │   │       │   ├── euc_jp.py
    │   │       │   ├── euc_kr.py
    │   │       │   ├── gb18030.py
    │   │       │   ├── gb2312.py
    │   │       │   ├── gbk.py
    │   │       │   ├── hex_codec.py
    │   │       │   ├── hp_roman8.py
    │   │       │   ├── hz.py
    │   │       │   ├── idna.py
    │   │       │   ├── __init__.py
    │   │       │   ├── iso2022_jp_1.py
    │   │       │   ├── iso2022_jp_2004.py
    │   │       │   ├── iso2022_jp_2.py
    │   │       │   ├── iso2022_jp_3.py
    │   │       │   ├── iso2022_jp_ext.py
    │   │       │   ├── iso2022_jp.py
    │   │       │   ├── iso2022_kr.py
    │   │       │   ├── iso8859_10.py
    │   │       │   ├── iso8859_11.py
    │   │       │   ├── iso8859_13.py
    │   │       │   ├── iso8859_14.py
    │   │       │   ├── iso8859_15.py
    │   │       │   ├── iso8859_16.py
    │   │       │   ├── iso8859_1.py
    │   │       │   ├── iso8859_2.py
    │   │       │   ├── iso8859_3.py
    │   │       │   ├── iso8859_4.py
    │   │       │   ├── iso8859_5.py
    │   │       │   ├── iso8859_6.py
    │   │       │   ├── iso8859_7.py
    │   │       │   ├── iso8859_8.py
    │   │       │   ├── iso8859_9.py
    │   │       │   ├── johab.py
    │   │       │   ├── koi8_r.py
    │   │       │   ├── koi8_t.py
    │   │       │   ├── koi8_u.py
    │   │       │   ├── kz1048.py
    │   │       │   ├── latin_1.py
    │   │       │   ├── mac_arabic.py
    │   │       │   ├── mac_croatian.py
    │   │       │   ├── mac_cyrillic.py
    │   │       │   ├── mac_farsi.py
    │   │       │   ├── mac_greek.py
    │   │       │   ├── mac_iceland.py
    │   │       │   ├── mac_latin2.py
    │   │       │   ├── mac_romanian.py
    │   │       │   ├── mac_roman.py
    │   │       │   ├── mac_turkish.py
    │   │       │   ├── mbcs.py
    │   │       │   ├── oem.py
    │   │       │   ├── palmos.py
    │   │       │   ├── ptcp154.py
    │   │       │   ├── punycode.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── aliases.cpython-311.opt-1.pyc
    │   │       │   │   ├── aliases.cpython-311.opt-2.pyc
    │   │       │   │   ├── aliases.cpython-311.pyc
    │   │       │   │   ├── ascii.cpython-311.opt-1.pyc
    │   │       │   │   ├── ascii.cpython-311.opt-2.pyc
    │   │       │   │   ├── ascii.cpython-311.pyc
    │   │       │   │   ├── base64_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── base64_codec.cpython-311.opt-2.pyc
    │   │       │   │   ├── base64_codec.cpython-311.pyc
    │   │       │   │   ├── big5.cpython-311.opt-1.pyc
    │   │       │   │   ├── big5.cpython-311.opt-2.pyc
    │   │       │   │   ├── big5.cpython-311.pyc
    │   │       │   │   ├── big5hkscs.cpython-311.opt-1.pyc
    │   │       │   │   ├── big5hkscs.cpython-311.opt-2.pyc
    │   │       │   │   ├── big5hkscs.cpython-311.pyc
    │   │       │   │   ├── bz2_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── bz2_codec.cpython-311.opt-2.pyc
    │   │       │   │   ├── bz2_codec.cpython-311.pyc
    │   │       │   │   ├── charmap.cpython-311.opt-1.pyc
    │   │       │   │   ├── charmap.cpython-311.opt-2.pyc
    │   │       │   │   ├── charmap.cpython-311.pyc
    │   │       │   │   ├── cp037.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp037.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp037.cpython-311.pyc
    │   │       │   │   ├── cp1006.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1006.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1006.cpython-311.pyc
    │   │       │   │   ├── cp1026.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1026.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1026.cpython-311.pyc
    │   │       │   │   ├── cp1125.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1125.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1125.cpython-311.pyc
    │   │       │   │   ├── cp1140.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1140.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1140.cpython-311.pyc
    │   │       │   │   ├── cp1250.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1250.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1250.cpython-311.pyc
    │   │       │   │   ├── cp1251.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1251.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1251.cpython-311.pyc
    │   │       │   │   ├── cp1252.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1252.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1252.cpython-311.pyc
    │   │       │   │   ├── cp1253.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1253.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1253.cpython-311.pyc
    │   │       │   │   ├── cp1254.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1254.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1254.cpython-311.pyc
    │   │       │   │   ├── cp1255.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1255.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1255.cpython-311.pyc
    │   │       │   │   ├── cp1256.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1256.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1256.cpython-311.pyc
    │   │       │   │   ├── cp1257.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1257.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1257.cpython-311.pyc
    │   │       │   │   ├── cp1258.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp1258.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp1258.cpython-311.pyc
    │   │       │   │   ├── cp273.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp273.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp273.cpython-311.pyc
    │   │       │   │   ├── cp424.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp424.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp424.cpython-311.pyc
    │   │       │   │   ├── cp437.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp437.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp437.cpython-311.pyc
    │   │       │   │   ├── cp500.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp500.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp500.cpython-311.pyc
    │   │       │   │   ├── cp720.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp720.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp720.cpython-311.pyc
    │   │       │   │   ├── cp737.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp737.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp737.cpython-311.pyc
    │   │       │   │   ├── cp775.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp775.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp775.cpython-311.pyc
    │   │       │   │   ├── cp850.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp850.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp850.cpython-311.pyc
    │   │       │   │   ├── cp852.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp852.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp852.cpython-311.pyc
    │   │       │   │   ├── cp855.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp855.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp855.cpython-311.pyc
    │   │       │   │   ├── cp856.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp856.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp856.cpython-311.pyc
    │   │       │   │   ├── cp857.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp857.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp857.cpython-311.pyc
    │   │       │   │   ├── cp858.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp858.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp858.cpython-311.pyc
    │   │       │   │   ├── cp860.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp860.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp860.cpython-311.pyc
    │   │       │   │   ├── cp861.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp861.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp861.cpython-311.pyc
    │   │       │   │   ├── cp862.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp862.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp862.cpython-311.pyc
    │   │       │   │   ├── cp863.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp863.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp863.cpython-311.pyc
    │   │       │   │   ├── cp864.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp864.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp864.cpython-311.pyc
    │   │       │   │   ├── cp865.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp865.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp865.cpython-311.pyc
    │   │       │   │   ├── cp866.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp866.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp866.cpython-311.pyc
    │   │       │   │   ├── cp869.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp869.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp869.cpython-311.pyc
    │   │       │   │   ├── cp874.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp874.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp874.cpython-311.pyc
    │   │       │   │   ├── cp875.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp875.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp875.cpython-311.pyc
    │   │       │   │   ├── cp932.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp932.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp932.cpython-311.pyc
    │   │       │   │   ├── cp949.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp949.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp949.cpython-311.pyc
    │   │       │   │   ├── cp950.cpython-311.opt-1.pyc
    │   │       │   │   ├── cp950.cpython-311.opt-2.pyc
    │   │       │   │   ├── cp950.cpython-311.pyc
    │   │       │   │   ├── euc_jis_2004.cpython-311.opt-1.pyc
    │   │       │   │   ├── euc_jis_2004.cpython-311.opt-2.pyc
    │   │       │   │   ├── euc_jis_2004.cpython-311.pyc
    │   │       │   │   ├── euc_jisx0213.cpython-311.opt-1.pyc
    │   │       │   │   ├── euc_jisx0213.cpython-311.opt-2.pyc
    │   │       │   │   ├── euc_jisx0213.cpython-311.pyc
    │   │       │   │   ├── euc_jp.cpython-311.opt-1.pyc
    │   │       │   │   ├── euc_jp.cpython-311.opt-2.pyc
    │   │       │   │   ├── euc_jp.cpython-311.pyc
    │   │       │   │   ├── euc_kr.cpython-311.opt-1.pyc
    │   │       │   │   ├── euc_kr.cpython-311.opt-2.pyc
    │   │       │   │   ├── euc_kr.cpython-311.pyc
    │   │       │   │   ├── gb18030.cpython-311.opt-1.pyc
    │   │       │   │   ├── gb18030.cpython-311.opt-2.pyc
    │   │       │   │   ├── gb18030.cpython-311.pyc
    │   │       │   │   ├── gb2312.cpython-311.opt-1.pyc
    │   │       │   │   ├── gb2312.cpython-311.opt-2.pyc
    │   │       │   │   ├── gb2312.cpython-311.pyc
    │   │       │   │   ├── gbk.cpython-311.opt-1.pyc
    │   │       │   │   ├── gbk.cpython-311.opt-2.pyc
    │   │       │   │   ├── gbk.cpython-311.pyc
    │   │       │   │   ├── hex_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── hex_codec.cpython-311.opt-2.pyc
    │   │       │   │   ├── hex_codec.cpython-311.pyc
    │   │       │   │   ├── hp_roman8.cpython-311.opt-1.pyc
    │   │       │   │   ├── hp_roman8.cpython-311.opt-2.pyc
    │   │       │   │   ├── hp_roman8.cpython-311.pyc
    │   │       │   │   ├── hz.cpython-311.opt-1.pyc
    │   │       │   │   ├── hz.cpython-311.opt-2.pyc
    │   │       │   │   ├── hz.cpython-311.pyc
    │   │       │   │   ├── idna.cpython-311.opt-1.pyc
    │   │       │   │   ├── idna.cpython-311.opt-2.pyc
    │   │       │   │   ├── idna.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp_1.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp_1.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp_1.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp_2004.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp_2004.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp_2004.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp_2.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp_2.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp_2.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp_3.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp_3.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp_3.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp.cpython-311.pyc
    │   │       │   │   ├── iso2022_jp_ext.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_jp_ext.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_jp_ext.cpython-311.pyc
    │   │       │   │   ├── iso2022_kr.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso2022_kr.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso2022_kr.cpython-311.pyc
    │   │       │   │   ├── iso8859_10.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_10.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_10.cpython-311.pyc
    │   │       │   │   ├── iso8859_11.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_11.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_11.cpython-311.pyc
    │   │       │   │   ├── iso8859_13.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_13.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_13.cpython-311.pyc
    │   │       │   │   ├── iso8859_14.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_14.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_14.cpython-311.pyc
    │   │       │   │   ├── iso8859_15.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_15.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_15.cpython-311.pyc
    │   │       │   │   ├── iso8859_16.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_16.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_16.cpython-311.pyc
    │   │       │   │   ├── iso8859_1.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_1.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_1.cpython-311.pyc
    │   │       │   │   ├── iso8859_2.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_2.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_2.cpython-311.pyc
    │   │       │   │   ├── iso8859_3.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_3.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_3.cpython-311.pyc
    │   │       │   │   ├── iso8859_4.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_4.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_4.cpython-311.pyc
    │   │       │   │   ├── iso8859_5.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_5.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_5.cpython-311.pyc
    │   │       │   │   ├── iso8859_6.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_6.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_6.cpython-311.pyc
    │   │       │   │   ├── iso8859_7.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_7.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_7.cpython-311.pyc
    │   │       │   │   ├── iso8859_8.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_8.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_8.cpython-311.pyc
    │   │       │   │   ├── iso8859_9.cpython-311.opt-1.pyc
    │   │       │   │   ├── iso8859_9.cpython-311.opt-2.pyc
    │   │       │   │   ├── iso8859_9.cpython-311.pyc
    │   │       │   │   ├── johab.cpython-311.opt-1.pyc
    │   │       │   │   ├── johab.cpython-311.opt-2.pyc
    │   │       │   │   ├── johab.cpython-311.pyc
    │   │       │   │   ├── koi8_r.cpython-311.opt-1.pyc
    │   │       │   │   ├── koi8_r.cpython-311.opt-2.pyc
    │   │       │   │   ├── koi8_r.cpython-311.pyc
    │   │       │   │   ├── koi8_t.cpython-311.opt-1.pyc
    │   │       │   │   ├── koi8_t.cpython-311.opt-2.pyc
    │   │       │   │   ├── koi8_t.cpython-311.pyc
    │   │       │   │   ├── koi8_u.cpython-311.opt-1.pyc
    │   │       │   │   ├── koi8_u.cpython-311.opt-2.pyc
    │   │       │   │   ├── koi8_u.cpython-311.pyc
    │   │       │   │   ├── kz1048.cpython-311.opt-1.pyc
    │   │       │   │   ├── kz1048.cpython-311.opt-2.pyc
    │   │       │   │   ├── kz1048.cpython-311.pyc
    │   │       │   │   ├── latin_1.cpython-311.opt-1.pyc
    │   │       │   │   ├── latin_1.cpython-311.opt-2.pyc
    │   │       │   │   ├── latin_1.cpython-311.pyc
    │   │       │   │   ├── mac_arabic.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_arabic.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_arabic.cpython-311.pyc
    │   │       │   │   ├── mac_croatian.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_croatian.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_croatian.cpython-311.pyc
    │   │       │   │   ├── mac_cyrillic.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_cyrillic.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_cyrillic.cpython-311.pyc
    │   │       │   │   ├── mac_farsi.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_farsi.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_farsi.cpython-311.pyc
    │   │       │   │   ├── mac_greek.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_greek.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_greek.cpython-311.pyc
    │   │       │   │   ├── mac_iceland.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_iceland.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_iceland.cpython-311.pyc
    │   │       │   │   ├── mac_latin2.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_latin2.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_latin2.cpython-311.pyc
    │   │       │   │   ├── mac_roman.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_roman.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_roman.cpython-311.pyc
    │   │       │   │   ├── mac_romanian.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_romanian.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_romanian.cpython-311.pyc
    │   │       │   │   ├── mac_turkish.cpython-311.opt-1.pyc
    │   │       │   │   ├── mac_turkish.cpython-311.opt-2.pyc
    │   │       │   │   ├── mac_turkish.cpython-311.pyc
    │   │       │   │   ├── mbcs.cpython-311.opt-1.pyc
    │   │       │   │   ├── mbcs.cpython-311.opt-2.pyc
    │   │       │   │   ├── mbcs.cpython-311.pyc
    │   │       │   │   ├── oem.cpython-311.opt-1.pyc
    │   │       │   │   ├── oem.cpython-311.opt-2.pyc
    │   │       │   │   ├── oem.cpython-311.pyc
    │   │       │   │   ├── palmos.cpython-311.opt-1.pyc
    │   │       │   │   ├── palmos.cpython-311.opt-2.pyc
    │   │       │   │   ├── palmos.cpython-311.pyc
    │   │       │   │   ├── ptcp154.cpython-311.opt-1.pyc
    │   │       │   │   ├── ptcp154.cpython-311.opt-2.pyc
    │   │       │   │   ├── ptcp154.cpython-311.pyc
    │   │       │   │   ├── punycode.cpython-311.opt-1.pyc
    │   │       │   │   ├── punycode.cpython-311.opt-2.pyc
    │   │       │   │   ├── punycode.cpython-311.pyc
    │   │       │   │   ├── quopri_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── quopri_codec.cpython-311.opt-2.pyc
    │   │       │   │   ├── quopri_codec.cpython-311.pyc
    │   │       │   │   ├── raw_unicode_escape.cpython-311.opt-1.pyc
    │   │       │   │   ├── raw_unicode_escape.cpython-311.opt-2.pyc
    │   │       │   │   ├── raw_unicode_escape.cpython-311.pyc
    │   │       │   │   ├── rot_13.cpython-311.opt-1.pyc
    │   │       │   │   ├── rot_13.cpython-311.opt-2.pyc
    │   │       │   │   ├── rot_13.cpython-311.pyc
    │   │       │   │   ├── shift_jis_2004.cpython-311.opt-1.pyc
    │   │       │   │   ├── shift_jis_2004.cpython-311.opt-2.pyc
    │   │       │   │   ├── shift_jis_2004.cpython-311.pyc
    │   │       │   │   ├── shift_jis.cpython-311.opt-1.pyc
    │   │       │   │   ├── shift_jis.cpython-311.opt-2.pyc
    │   │       │   │   ├── shift_jis.cpython-311.pyc
    │   │       │   │   ├── shift_jisx0213.cpython-311.opt-1.pyc
    │   │       │   │   ├── shift_jisx0213.cpython-311.opt-2.pyc
    │   │       │   │   ├── shift_jisx0213.cpython-311.pyc
    │   │       │   │   ├── tis_620.cpython-311.opt-1.pyc
    │   │       │   │   ├── tis_620.cpython-311.opt-2.pyc
    │   │       │   │   ├── tis_620.cpython-311.pyc
    │   │       │   │   ├── undefined.cpython-311.opt-1.pyc
    │   │       │   │   ├── undefined.cpython-311.opt-2.pyc
    │   │       │   │   ├── undefined.cpython-311.pyc
    │   │       │   │   ├── unicode_escape.cpython-311.opt-1.pyc
    │   │       │   │   ├── unicode_escape.cpython-311.opt-2.pyc
    │   │       │   │   ├── unicode_escape.cpython-311.pyc
    │   │       │   │   ├── utf_16_be.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_16_be.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_16_be.cpython-311.pyc
    │   │       │   │   ├── utf_16.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_16.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_16.cpython-311.pyc
    │   │       │   │   ├── utf_16_le.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_16_le.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_16_le.cpython-311.pyc
    │   │       │   │   ├── utf_32_be.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_32_be.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_32_be.cpython-311.pyc
    │   │       │   │   ├── utf_32.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_32.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_32.cpython-311.pyc
    │   │       │   │   ├── utf_32_le.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_32_le.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_32_le.cpython-311.pyc
    │   │       │   │   ├── utf_7.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_7.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_7.cpython-311.pyc
    │   │       │   │   ├── utf_8.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_8.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_8.cpython-311.pyc
    │   │       │   │   ├── utf_8_sig.cpython-311.opt-1.pyc
    │   │       │   │   ├── utf_8_sig.cpython-311.opt-2.pyc
    │   │       │   │   ├── utf_8_sig.cpython-311.pyc
    │   │       │   │   ├── uu_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── uu_codec.cpython-311.opt-2.pyc
    │   │       │   │   ├── uu_codec.cpython-311.pyc
    │   │       │   │   ├── zlib_codec.cpython-311.opt-1.pyc
    │   │       │   │   ├── zlib_codec.cpython-311.opt-2.pyc
    │   │       │   │   └── zlib_codec.cpython-311.pyc
    │   │       │   ├── quopri_codec.py
    │   │       │   ├── raw_unicode_escape.py
    │   │       │   ├── rot_13.py
    │   │       │   ├── shift_jis_2004.py
    │   │       │   ├── shift_jis.py
    │   │       │   ├── shift_jisx0213.py
    │   │       │   ├── tis_620.py
    │   │       │   ├── undefined.py
    │   │       │   ├── unicode_escape.py
    │   │       │   ├── utf_16_be.py
    │   │       │   ├── utf_16_le.py
    │   │       │   ├── utf_16.py
    │   │       │   ├── utf_32_be.py
    │   │       │   ├── utf_32_le.py
    │   │       │   ├── utf_32.py
    │   │       │   ├── utf_7.py
    │   │       │   ├── utf_8.py
    │   │       │   ├── utf_8_sig.py
    │   │       │   ├── uu_codec.py
    │   │       │   └── zlib_codec.py
    │   │       ├── ensurepip
    │   │       │   ├── _bundled
    │   │       │   │   ├── pip-23.1.2-py3-none-any.whl
    │   │       │   │   └── setuptools-65.5.0-py3-none-any.whl
    │   │       │   ├── __init__.py
    │   │       │   ├── __main__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── _uninstall.cpython-311.opt-1.pyc
    │   │       │   │   ├── _uninstall.cpython-311.opt-2.pyc
    │   │       │   │   └── _uninstall.cpython-311.pyc
    │   │       │   └── _uninstall.py
    │   │       ├── enum.py
    │   │       ├── filecmp.py
    │   │       ├── fileinput.py
    │   │       ├── fnmatch.py
    │   │       ├── fractions.py
    │   │       ├── ftplib.py
    │   │       ├── functools.py
    │   │       ├── __future__.py
    │   │       ├── genericpath.py
    │   │       ├── getopt.py
    │   │       ├── getpass.py
    │   │       ├── gettext.py
    │   │       ├── glob.py
    │   │       ├── graphlib.py
    │   │       ├── gzip.py
    │   │       ├── hashlib.py
    │   │       ├── heapq.py
    │   │       ├── __hello__.py
    │   │       ├── hmac.py
    │   │       ├── html
    │   │       │   ├── entities.py
    │   │       │   ├── __init__.py
    │   │       │   ├── parser.py
    │   │       │   └── __pycache__
    │   │       │       ├── entities.cpython-311.opt-1.pyc
    │   │       │       ├── entities.cpython-311.opt-2.pyc
    │   │       │       ├── entities.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       ├── __init__.cpython-311.pyc
    │   │       │       ├── parser.cpython-311.opt-1.pyc
    │   │       │       ├── parser.cpython-311.opt-2.pyc
    │   │       │       └── parser.cpython-311.pyc
    │   │       ├── http
    │   │       │   ├── client.py
    │   │       │   ├── cookiejar.py
    │   │       │   ├── cookies.py
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── client.cpython-311.opt-1.pyc
    │   │       │   │   ├── client.cpython-311.opt-2.pyc
    │   │       │   │   ├── client.cpython-311.pyc
    │   │       │   │   ├── cookiejar.cpython-311.opt-1.pyc
    │   │       │   │   ├── cookiejar.cpython-311.opt-2.pyc
    │   │       │   │   ├── cookiejar.cpython-311.pyc
    │   │       │   │   ├── cookies.cpython-311.opt-1.pyc
    │   │       │   │   ├── cookies.cpython-311.opt-2.pyc
    │   │       │   │   ├── cookies.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── server.cpython-311.opt-1.pyc
    │   │       │   │   ├── server.cpython-311.opt-2.pyc
    │   │       │   │   └── server.cpython-311.pyc
    │   │       │   └── server.py
    │   │       ├── idlelib
    │   │       │   ├── autocomplete.py
    │   │       │   ├── autocomplete_w.py
    │   │       │   ├── autoexpand.py
    │   │       │   ├── browser.py
    │   │       │   ├── calltip.py
    │   │       │   ├── calltip_w.py
    │   │       │   ├── ChangeLog
    │   │       │   ├── codecontext.py
    │   │       │   ├── colorizer.py
    │   │       │   ├── configdialog.py
    │   │       │   ├── config-extensions.def
    │   │       │   ├── config-highlight.def
    │   │       │   ├── config_key.py
    │   │       │   ├── config-keys.def
    │   │       │   ├── config-main.def
    │   │       │   ├── config.py
    │   │       │   ├── CREDITS.txt
    │   │       │   ├── debugger.py
    │   │       │   ├── debugger_r.py
    │   │       │   ├── debugobj.py
    │   │       │   ├── debugobj_r.py
    │   │       │   ├── delegator.py
    │   │       │   ├── dynoption.py
    │   │       │   ├── editor.py
    │   │       │   ├── extend.txt
    │   │       │   ├── filelist.py
    │   │       │   ├── format.py
    │   │       │   ├── grep.py
    │   │       │   ├── help_about.py
    │   │       │   ├── help.html
    │   │       │   ├── help.py
    │   │       │   ├── history.py
    │   │       │   ├── HISTORY.txt
    │   │       │   ├── hyperparser.py
    │   │       │   ├── Icons
    │   │       │   │   ├── folder.gif
    │   │       │   │   ├── idle_16.gif
    │   │       │   │   ├── idle_16.png
    │   │       │   │   ├── idle_256.png
    │   │       │   │   ├── idle_32.gif
    │   │       │   │   ├── idle_32.png
    │   │       │   │   ├── idle_48.gif
    │   │       │   │   ├── idle_48.png
    │   │       │   │   ├── idle.ico
    │   │       │   │   ├── minusnode.gif
    │   │       │   │   ├── openfolder.gif
    │   │       │   │   ├── plusnode.gif
    │   │       │   │   ├── python.gif
    │   │       │   │   ├── README.txt
    │   │       │   │   └── tk.gif
    │   │       │   ├── idle.bat
    │   │       │   ├── idle.py
    │   │       │   ├── idle.pyw
    │   │       │   ├── idle_test
    │   │       │   │   ├── example_noext
    │   │       │   │   ├── example_stub.pyi
    │   │       │   │   ├── htest.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── mock_idle.py
    │   │       │   │   ├── mock_tk.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── htest.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── htest.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── htest.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── mock_idle.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── mock_idle.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── mock_idle.cpython-311.pyc
    │   │       │   │   │   ├── mock_tk.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── mock_tk.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── mock_tk.cpython-311.pyc
    │   │       │   │   │   ├── template.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── template.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── template.cpython-311.pyc
    │   │       │   │   │   ├── test_autocomplete.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_autocomplete.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_autocomplete.cpython-311.pyc
    │   │       │   │   │   ├── test_autocomplete_w.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_autocomplete_w.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_autocomplete_w.cpython-311.pyc
    │   │       │   │   │   ├── test_autoexpand.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_autoexpand.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_autoexpand.cpython-311.pyc
    │   │       │   │   │   ├── test_browser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_browser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_browser.cpython-311.pyc
    │   │       │   │   │   ├── test_calltip.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_calltip.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_calltip.cpython-311.pyc
    │   │       │   │   │   ├── test_calltip_w.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_calltip_w.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_calltip_w.cpython-311.pyc
    │   │       │   │   │   ├── test_codecontext.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_codecontext.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_codecontext.cpython-311.pyc
    │   │       │   │   │   ├── test_colorizer.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_colorizer.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_colorizer.cpython-311.pyc
    │   │       │   │   │   ├── test_config.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_config.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_config.cpython-311.pyc
    │   │       │   │   │   ├── test_configdialog.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_configdialog.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_configdialog.cpython-311.pyc
    │   │       │   │   │   ├── test_config_key.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_config_key.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_config_key.cpython-311.pyc
    │   │       │   │   │   ├── test_debugger.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_debugger.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_debugger.cpython-311.pyc
    │   │       │   │   │   ├── test_debugger_r.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_debugger_r.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_debugger_r.cpython-311.pyc
    │   │       │   │   │   ├── test_debugobj.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_debugobj.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_debugobj.cpython-311.pyc
    │   │       │   │   │   ├── test_debugobj_r.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_debugobj_r.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_debugobj_r.cpython-311.pyc
    │   │       │   │   │   ├── test_delegator.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_delegator.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_delegator.cpython-311.pyc
    │   │       │   │   │   ├── test_editmenu.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_editmenu.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_editmenu.cpython-311.pyc
    │   │       │   │   │   ├── test_editor.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_editor.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_editor.cpython-311.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_filelist.cpython-311.pyc
    │   │       │   │   │   ├── test_format.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_format.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_format.cpython-311.pyc
    │   │       │   │   │   ├── test_grep.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_grep.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_grep.cpython-311.pyc
    │   │       │   │   │   ├── test_help_about.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_help_about.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_help_about.cpython-311.pyc
    │   │       │   │   │   ├── test_help.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_help.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_help.cpython-311.pyc
    │   │       │   │   │   ├── test_history.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_history.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_history.cpython-311.pyc
    │   │       │   │   │   ├── test_hyperparser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_hyperparser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_hyperparser.cpython-311.pyc
    │   │       │   │   │   ├── test_iomenu.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_iomenu.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_iomenu.cpython-311.pyc
    │   │       │   │   │   ├── test_macosx.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_macosx.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_macosx.cpython-311.pyc
    │   │       │   │   │   ├── test_mainmenu.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_mainmenu.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_mainmenu.cpython-311.pyc
    │   │       │   │   │   ├── test_multicall.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_multicall.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_multicall.cpython-311.pyc
    │   │       │   │   │   ├── test_outwin.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_outwin.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_outwin.cpython-311.pyc
    │   │       │   │   │   ├── test_parenmatch.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_parenmatch.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_parenmatch.cpython-311.pyc
    │   │       │   │   │   ├── test_pathbrowser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pathbrowser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pathbrowser.cpython-311.pyc
    │   │       │   │   │   ├── test_percolator.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_percolator.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_percolator.cpython-311.pyc
    │   │       │   │   │   ├── test_pyparse.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pyparse.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pyparse.cpython-311.pyc
    │   │       │   │   │   ├── test_pyshell.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pyshell.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pyshell.cpython-311.pyc
    │   │       │   │   │   ├── test_query.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_query.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_query.cpython-311.pyc
    │   │       │   │   │   ├── test_redirector.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_redirector.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_redirector.cpython-311.pyc
    │   │       │   │   │   ├── test_replace.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_replace.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_replace.cpython-311.pyc
    │   │       │   │   │   ├── test_rpc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_rpc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_rpc.cpython-311.pyc
    │   │       │   │   │   ├── test_run.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_run.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_run.cpython-311.pyc
    │   │       │   │   │   ├── test_runscript.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_runscript.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_runscript.cpython-311.pyc
    │   │       │   │   │   ├── test_scrolledlist.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_scrolledlist.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_scrolledlist.cpython-311.pyc
    │   │       │   │   │   ├── test_searchbase.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_searchbase.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_searchbase.cpython-311.pyc
    │   │       │   │   │   ├── test_search.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_search.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_search.cpython-311.pyc
    │   │       │   │   │   ├── test_searchengine.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_searchengine.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_searchengine.cpython-311.pyc
    │   │       │   │   │   ├── test_sidebar.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sidebar.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sidebar.cpython-311.pyc
    │   │       │   │   │   ├── test_squeezer.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_squeezer.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_squeezer.cpython-311.pyc
    │   │       │   │   │   ├── test_stackviewer.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_stackviewer.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_stackviewer.cpython-311.pyc
    │   │       │   │   │   ├── test_statusbar.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_statusbar.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_statusbar.cpython-311.pyc
    │   │       │   │   │   ├── test_text.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_text.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_text.cpython-311.pyc
    │   │       │   │   │   ├── test_textview.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_textview.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_textview.cpython-311.pyc
    │   │       │   │   │   ├── test_tooltip.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_tooltip.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_tooltip.cpython-311.pyc
    │   │       │   │   │   ├── test_tree.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_tree.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_tree.cpython-311.pyc
    │   │       │   │   │   ├── test_undo.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_undo.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_undo.cpython-311.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_util.cpython-311.pyc
    │   │       │   │   │   ├── test_warning.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_warning.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_warning.cpython-311.pyc
    │   │       │   │   │   ├── test_window.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_window.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_window.cpython-311.pyc
    │   │       │   │   │   ├── test_zoomheight.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_zoomheight.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_zoomheight.cpython-311.pyc
    │   │       │   │   │   ├── test_zzdummy.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_zzdummy.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_zzdummy.cpython-311.pyc
    │   │       │   │   │   ├── tkinter_testing_utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── tkinter_testing_utils.cpython-311.opt-2.pyc
    │   │       │   │   │   └── tkinter_testing_utils.cpython-311.pyc
    │   │       │   │   ├── README.txt
    │   │       │   │   ├── template.py
    │   │       │   │   ├── test_autocomplete.py
    │   │       │   │   ├── test_autocomplete_w.py
    │   │       │   │   ├── test_autoexpand.py
    │   │       │   │   ├── test_browser.py
    │   │       │   │   ├── test_calltip.py
    │   │       │   │   ├── test_calltip_w.py
    │   │       │   │   ├── test_codecontext.py
    │   │       │   │   ├── test_colorizer.py
    │   │       │   │   ├── test_configdialog.py
    │   │       │   │   ├── test_config_key.py
    │   │       │   │   ├── test_config.py
    │   │       │   │   ├── test_debugger.py
    │   │       │   │   ├── test_debugger_r.py
    │   │       │   │   ├── test_debugobj.py
    │   │       │   │   ├── test_debugobj_r.py
    │   │       │   │   ├── test_delegator.py
    │   │       │   │   ├── test_editmenu.py
    │   │       │   │   ├── test_editor.py
    │   │       │   │   ├── test_filelist.py
    │   │       │   │   ├── test_format.py
    │   │       │   │   ├── test_grep.py
    │   │       │   │   ├── test_help_about.py
    │   │       │   │   ├── test_help.py
    │   │       │   │   ├── test_history.py
    │   │       │   │   ├── test_hyperparser.py
    │   │       │   │   ├── test_iomenu.py
    │   │       │   │   ├── test_macosx.py
    │   │       │   │   ├── test_mainmenu.py
    │   │       │   │   ├── test_multicall.py
    │   │       │   │   ├── test_outwin.py
    │   │       │   │   ├── test_parenmatch.py
    │   │       │   │   ├── test_pathbrowser.py
    │   │       │   │   ├── test_percolator.py
    │   │       │   │   ├── test_pyparse.py
    │   │       │   │   ├── test_pyshell.py
    │   │       │   │   ├── test_query.py
    │   │       │   │   ├── test_redirector.py
    │   │       │   │   ├── test_replace.py
    │   │       │   │   ├── test_rpc.py
    │   │       │   │   ├── test_run.py
    │   │       │   │   ├── test_runscript.py
    │   │       │   │   ├── test_scrolledlist.py
    │   │       │   │   ├── test_searchbase.py
    │   │       │   │   ├── test_searchengine.py
    │   │       │   │   ├── test_search.py
    │   │       │   │   ├── test_sidebar.py
    │   │       │   │   ├── test_squeezer.py
    │   │       │   │   ├── test_stackviewer.py
    │   │       │   │   ├── test_statusbar.py
    │   │       │   │   ├── test_text.py
    │   │       │   │   ├── test_textview.py
    │   │       │   │   ├── test_tooltip.py
    │   │       │   │   ├── test_tree.py
    │   │       │   │   ├── test_undo.py
    │   │       │   │   ├── test_util.py
    │   │       │   │   ├── test_warning.py
    │   │       │   │   ├── test_window.py
    │   │       │   │   ├── test_zoomheight.py
    │   │       │   │   ├── test_zzdummy.py
    │   │       │   │   └── tkinter_testing_utils.py
    │   │       │   ├── __init__.py
    │   │       │   ├── iomenu.py
    │   │       │   ├── macosx.py
    │   │       │   ├── mainmenu.py
    │   │       │   ├── __main__.py
    │   │       │   ├── multicall.py
    │   │       │   ├── NEWS2x.txt
    │   │       │   ├── NEWS.txt
    │   │       │   ├── outwin.py
    │   │       │   ├── parenmatch.py
    │   │       │   ├── pathbrowser.py
    │   │       │   ├── percolator.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── autocomplete.cpython-311.opt-1.pyc
    │   │       │   │   ├── autocomplete.cpython-311.opt-2.pyc
    │   │       │   │   ├── autocomplete.cpython-311.pyc
    │   │       │   │   ├── autocomplete_w.cpython-311.opt-1.pyc
    │   │       │   │   ├── autocomplete_w.cpython-311.opt-2.pyc
    │   │       │   │   ├── autocomplete_w.cpython-311.pyc
    │   │       │   │   ├── autoexpand.cpython-311.opt-1.pyc
    │   │       │   │   ├── autoexpand.cpython-311.opt-2.pyc
    │   │       │   │   ├── autoexpand.cpython-311.pyc
    │   │       │   │   ├── browser.cpython-311.opt-1.pyc
    │   │       │   │   ├── browser.cpython-311.opt-2.pyc
    │   │       │   │   ├── browser.cpython-311.pyc
    │   │       │   │   ├── calltip.cpython-311.opt-1.pyc
    │   │       │   │   ├── calltip.cpython-311.opt-2.pyc
    │   │       │   │   ├── calltip.cpython-311.pyc
    │   │       │   │   ├── calltip_w.cpython-311.opt-1.pyc
    │   │       │   │   ├── calltip_w.cpython-311.opt-2.pyc
    │   │       │   │   ├── calltip_w.cpython-311.pyc
    │   │       │   │   ├── codecontext.cpython-311.opt-1.pyc
    │   │       │   │   ├── codecontext.cpython-311.opt-2.pyc
    │   │       │   │   ├── codecontext.cpython-311.pyc
    │   │       │   │   ├── colorizer.cpython-311.opt-1.pyc
    │   │       │   │   ├── colorizer.cpython-311.opt-2.pyc
    │   │       │   │   ├── colorizer.cpython-311.pyc
    │   │       │   │   ├── config.cpython-311.opt-1.pyc
    │   │       │   │   ├── config.cpython-311.opt-2.pyc
    │   │       │   │   ├── config.cpython-311.pyc
    │   │       │   │   ├── configdialog.cpython-311.opt-1.pyc
    │   │       │   │   ├── configdialog.cpython-311.opt-2.pyc
    │   │       │   │   ├── configdialog.cpython-311.pyc
    │   │       │   │   ├── config_key.cpython-311.opt-1.pyc
    │   │       │   │   ├── config_key.cpython-311.opt-2.pyc
    │   │       │   │   ├── config_key.cpython-311.pyc
    │   │       │   │   ├── debugger.cpython-311.opt-1.pyc
    │   │       │   │   ├── debugger.cpython-311.opt-2.pyc
    │   │       │   │   ├── debugger.cpython-311.pyc
    │   │       │   │   ├── debugger_r.cpython-311.opt-1.pyc
    │   │       │   │   ├── debugger_r.cpython-311.opt-2.pyc
    │   │       │   │   ├── debugger_r.cpython-311.pyc
    │   │       │   │   ├── debugobj.cpython-311.opt-1.pyc
    │   │       │   │   ├── debugobj.cpython-311.opt-2.pyc
    │   │       │   │   ├── debugobj.cpython-311.pyc
    │   │       │   │   ├── debugobj_r.cpython-311.opt-1.pyc
    │   │       │   │   ├── debugobj_r.cpython-311.opt-2.pyc
    │   │       │   │   ├── debugobj_r.cpython-311.pyc
    │   │       │   │   ├── delegator.cpython-311.opt-1.pyc
    │   │       │   │   ├── delegator.cpython-311.opt-2.pyc
    │   │       │   │   ├── delegator.cpython-311.pyc
    │   │       │   │   ├── dynoption.cpython-311.opt-1.pyc
    │   │       │   │   ├── dynoption.cpython-311.opt-2.pyc
    │   │       │   │   ├── dynoption.cpython-311.pyc
    │   │       │   │   ├── editor.cpython-311.opt-1.pyc
    │   │       │   │   ├── editor.cpython-311.opt-2.pyc
    │   │       │   │   ├── editor.cpython-311.pyc
    │   │       │   │   ├── filelist.cpython-311.opt-1.pyc
    │   │       │   │   ├── filelist.cpython-311.opt-2.pyc
    │   │       │   │   ├── filelist.cpython-311.pyc
    │   │       │   │   ├── format.cpython-311.opt-1.pyc
    │   │       │   │   ├── format.cpython-311.opt-2.pyc
    │   │       │   │   ├── format.cpython-311.pyc
    │   │       │   │   ├── grep.cpython-311.opt-1.pyc
    │   │       │   │   ├── grep.cpython-311.opt-2.pyc
    │   │       │   │   ├── grep.cpython-311.pyc
    │   │       │   │   ├── help_about.cpython-311.opt-1.pyc
    │   │       │   │   ├── help_about.cpython-311.opt-2.pyc
    │   │       │   │   ├── help_about.cpython-311.pyc
    │   │       │   │   ├── help.cpython-311.opt-1.pyc
    │   │       │   │   ├── help.cpython-311.opt-2.pyc
    │   │       │   │   ├── help.cpython-311.pyc
    │   │       │   │   ├── history.cpython-311.opt-1.pyc
    │   │       │   │   ├── history.cpython-311.opt-2.pyc
    │   │       │   │   ├── history.cpython-311.pyc
    │   │       │   │   ├── hyperparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── hyperparser.cpython-311.opt-2.pyc
    │   │       │   │   ├── hyperparser.cpython-311.pyc
    │   │       │   │   ├── idle.cpython-311.opt-1.pyc
    │   │       │   │   ├── idle.cpython-311.opt-2.pyc
    │   │       │   │   ├── idle.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── iomenu.cpython-311.opt-1.pyc
    │   │       │   │   ├── iomenu.cpython-311.opt-2.pyc
    │   │       │   │   ├── iomenu.cpython-311.pyc
    │   │       │   │   ├── macosx.cpython-311.opt-1.pyc
    │   │       │   │   ├── macosx.cpython-311.opt-2.pyc
    │   │       │   │   ├── macosx.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── mainmenu.cpython-311.opt-1.pyc
    │   │       │   │   ├── mainmenu.cpython-311.opt-2.pyc
    │   │       │   │   ├── mainmenu.cpython-311.pyc
    │   │       │   │   ├── multicall.cpython-311.opt-1.pyc
    │   │       │   │   ├── multicall.cpython-311.opt-2.pyc
    │   │       │   │   ├── multicall.cpython-311.pyc
    │   │       │   │   ├── outwin.cpython-311.opt-1.pyc
    │   │       │   │   ├── outwin.cpython-311.opt-2.pyc
    │   │       │   │   ├── outwin.cpython-311.pyc
    │   │       │   │   ├── parenmatch.cpython-311.opt-1.pyc
    │   │       │   │   ├── parenmatch.cpython-311.opt-2.pyc
    │   │       │   │   ├── parenmatch.cpython-311.pyc
    │   │       │   │   ├── pathbrowser.cpython-311.opt-1.pyc
    │   │       │   │   ├── pathbrowser.cpython-311.opt-2.pyc
    │   │       │   │   ├── pathbrowser.cpython-311.pyc
    │   │       │   │   ├── percolator.cpython-311.opt-1.pyc
    │   │       │   │   ├── percolator.cpython-311.opt-2.pyc
    │   │       │   │   ├── percolator.cpython-311.pyc
    │   │       │   │   ├── pyparse.cpython-311.opt-1.pyc
    │   │       │   │   ├── pyparse.cpython-311.opt-2.pyc
    │   │       │   │   ├── pyparse.cpython-311.pyc
    │   │       │   │   ├── pyshell.cpython-311.opt-1.pyc
    │   │       │   │   ├── pyshell.cpython-311.opt-2.pyc
    │   │       │   │   ├── pyshell.cpython-311.pyc
    │   │       │   │   ├── query.cpython-311.opt-1.pyc
    │   │       │   │   ├── query.cpython-311.opt-2.pyc
    │   │       │   │   ├── query.cpython-311.pyc
    │   │       │   │   ├── redirector.cpython-311.opt-1.pyc
    │   │       │   │   ├── redirector.cpython-311.opt-2.pyc
    │   │       │   │   ├── redirector.cpython-311.pyc
    │   │       │   │   ├── replace.cpython-311.opt-1.pyc
    │   │       │   │   ├── replace.cpython-311.opt-2.pyc
    │   │       │   │   ├── replace.cpython-311.pyc
    │   │       │   │   ├── rpc.cpython-311.opt-1.pyc
    │   │       │   │   ├── rpc.cpython-311.opt-2.pyc
    │   │       │   │   ├── rpc.cpython-311.pyc
    │   │       │   │   ├── run.cpython-311.opt-1.pyc
    │   │       │   │   ├── run.cpython-311.opt-2.pyc
    │   │       │   │   ├── run.cpython-311.pyc
    │   │       │   │   ├── runscript.cpython-311.opt-1.pyc
    │   │       │   │   ├── runscript.cpython-311.opt-2.pyc
    │   │       │   │   ├── runscript.cpython-311.pyc
    │   │       │   │   ├── scrolledlist.cpython-311.opt-1.pyc
    │   │       │   │   ├── scrolledlist.cpython-311.opt-2.pyc
    │   │       │   │   ├── scrolledlist.cpython-311.pyc
    │   │       │   │   ├── searchbase.cpython-311.opt-1.pyc
    │   │       │   │   ├── searchbase.cpython-311.opt-2.pyc
    │   │       │   │   ├── searchbase.cpython-311.pyc
    │   │       │   │   ├── search.cpython-311.opt-1.pyc
    │   │       │   │   ├── search.cpython-311.opt-2.pyc
    │   │       │   │   ├── search.cpython-311.pyc
    │   │       │   │   ├── searchengine.cpython-311.opt-1.pyc
    │   │       │   │   ├── searchengine.cpython-311.opt-2.pyc
    │   │       │   │   ├── searchengine.cpython-311.pyc
    │   │       │   │   ├── sidebar.cpython-311.opt-1.pyc
    │   │       │   │   ├── sidebar.cpython-311.opt-2.pyc
    │   │       │   │   ├── sidebar.cpython-311.pyc
    │   │       │   │   ├── squeezer.cpython-311.opt-1.pyc
    │   │       │   │   ├── squeezer.cpython-311.opt-2.pyc
    │   │       │   │   ├── squeezer.cpython-311.pyc
    │   │       │   │   ├── stackviewer.cpython-311.opt-1.pyc
    │   │       │   │   ├── stackviewer.cpython-311.opt-2.pyc
    │   │       │   │   ├── stackviewer.cpython-311.pyc
    │   │       │   │   ├── statusbar.cpython-311.opt-1.pyc
    │   │       │   │   ├── statusbar.cpython-311.opt-2.pyc
    │   │       │   │   ├── statusbar.cpython-311.pyc
    │   │       │   │   ├── textview.cpython-311.opt-1.pyc
    │   │       │   │   ├── textview.cpython-311.opt-2.pyc
    │   │       │   │   ├── textview.cpython-311.pyc
    │   │       │   │   ├── tooltip.cpython-311.opt-1.pyc
    │   │       │   │   ├── tooltip.cpython-311.opt-2.pyc
    │   │       │   │   ├── tooltip.cpython-311.pyc
    │   │       │   │   ├── tree.cpython-311.opt-1.pyc
    │   │       │   │   ├── tree.cpython-311.opt-2.pyc
    │   │       │   │   ├── tree.cpython-311.pyc
    │   │       │   │   ├── undo.cpython-311.opt-1.pyc
    │   │       │   │   ├── undo.cpython-311.opt-2.pyc
    │   │       │   │   ├── undo.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   ├── util.cpython-311.pyc
    │   │       │   │   ├── window.cpython-311.opt-1.pyc
    │   │       │   │   ├── window.cpython-311.opt-2.pyc
    │   │       │   │   ├── window.cpython-311.pyc
    │   │       │   │   ├── zoomheight.cpython-311.opt-1.pyc
    │   │       │   │   ├── zoomheight.cpython-311.opt-2.pyc
    │   │       │   │   ├── zoomheight.cpython-311.pyc
    │   │       │   │   ├── zzdummy.cpython-311.opt-1.pyc
    │   │       │   │   ├── zzdummy.cpython-311.opt-2.pyc
    │   │       │   │   └── zzdummy.cpython-311.pyc
    │   │       │   ├── pyparse.py
    │   │       │   ├── pyshell.py
    │   │       │   ├── query.py
    │   │       │   ├── README.txt
    │   │       │   ├── redirector.py
    │   │       │   ├── replace.py
    │   │       │   ├── rpc.py
    │   │       │   ├── run.py
    │   │       │   ├── runscript.py
    │   │       │   ├── scrolledlist.py
    │   │       │   ├── searchbase.py
    │   │       │   ├── searchengine.py
    │   │       │   ├── search.py
    │   │       │   ├── sidebar.py
    │   │       │   ├── squeezer.py
    │   │       │   ├── stackviewer.py
    │   │       │   ├── statusbar.py
    │   │       │   ├── textview.py
    │   │       │   ├── TODO.txt
    │   │       │   ├── tooltip.py
    │   │       │   ├── tree.py
    │   │       │   ├── undo.py
    │   │       │   ├── util.py
    │   │       │   ├── window.py
    │   │       │   ├── zoomheight.py
    │   │       │   └── zzdummy.py
    │   │       ├── imaplib.py
    │   │       ├── imghdr.py
    │   │       ├── importlib
    │   │       │   ├── _abc.py
    │   │       │   ├── abc.py
    │   │       │   ├── _bootstrap_external.py
    │   │       │   ├── _bootstrap.py
    │   │       │   ├── __init__.py
    │   │       │   ├── machinery.py
    │   │       │   ├── metadata
    │   │       │   │   ├── _adapters.py
    │   │       │   │   ├── _collections.py
    │   │       │   │   ├── _functools.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── _itertools.py
    │   │       │   │   ├── _meta.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── _adapters.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _adapters.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _adapters.cpython-311.pyc
    │   │       │   │   │   ├── _collections.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _collections.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _collections.cpython-311.pyc
    │   │       │   │   │   ├── _functools.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _functools.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _functools.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │   │   ├── _meta.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _meta.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _meta.cpython-311.pyc
    │   │       │   │   │   ├── _text.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _text.cpython-311.opt-2.pyc
    │   │       │   │   │   └── _text.cpython-311.pyc
    │   │       │   │   └── _text.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── _abc.cpython-311.opt-1.pyc
    │   │       │   │   ├── abc.cpython-311.opt-1.pyc
    │   │       │   │   ├── _abc.cpython-311.opt-2.pyc
    │   │       │   │   ├── abc.cpython-311.opt-2.pyc
    │   │       │   │   ├── _abc.cpython-311.pyc
    │   │       │   │   ├── abc.cpython-311.pyc
    │   │       │   │   ├── _bootstrap.cpython-311.opt-1.pyc
    │   │       │   │   ├── _bootstrap.cpython-311.opt-2.pyc
    │   │       │   │   ├── _bootstrap.cpython-311.pyc
    │   │       │   │   ├── _bootstrap_external.cpython-311.opt-1.pyc
    │   │       │   │   ├── _bootstrap_external.cpython-311.opt-2.pyc
    │   │       │   │   ├── _bootstrap_external.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── machinery.cpython-311.opt-1.pyc
    │   │       │   │   ├── machinery.cpython-311.opt-2.pyc
    │   │       │   │   ├── machinery.cpython-311.pyc
    │   │       │   │   ├── readers.cpython-311.opt-1.pyc
    │   │       │   │   ├── readers.cpython-311.opt-2.pyc
    │   │       │   │   ├── readers.cpython-311.pyc
    │   │       │   │   ├── simple.cpython-311.opt-1.pyc
    │   │       │   │   ├── simple.cpython-311.opt-2.pyc
    │   │       │   │   ├── simple.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   └── util.cpython-311.pyc
    │   │       │   ├── readers.py
    │   │       │   ├── resources
    │   │       │   │   ├── abc.py
    │   │       │   │   ├── _adapters.py
    │   │       │   │   ├── _common.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── _itertools.py
    │   │       │   │   ├── _legacy.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── abc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── abc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── abc.cpython-311.pyc
    │   │       │   │   │   ├── _adapters.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _adapters.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _adapters.cpython-311.pyc
    │   │       │   │   │   ├── _common.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _common.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _common.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │   │   ├── _legacy.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _legacy.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _legacy.cpython-311.pyc
    │   │       │   │   │   ├── readers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── readers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── readers.cpython-311.pyc
    │   │       │   │   │   ├── simple.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── simple.cpython-311.opt-2.pyc
    │   │       │   │   │   └── simple.cpython-311.pyc
    │   │       │   │   ├── readers.py
    │   │       │   │   └── simple.py
    │   │       │   ├── simple.py
    │   │       │   └── util.py
    │   │       ├── imp.py
    │   │       ├── inspect.py
    │   │       ├── io.py
    │   │       ├── ipaddress.py
    │   │       ├── json
    │   │       │   ├── decoder.py
    │   │       │   ├── encoder.py
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── decoder.cpython-311.opt-1.pyc
    │   │       │   │   ├── decoder.cpython-311.opt-2.pyc
    │   │       │   │   ├── decoder.cpython-311.pyc
    │   │       │   │   ├── encoder.cpython-311.opt-1.pyc
    │   │       │   │   ├── encoder.cpython-311.opt-2.pyc
    │   │       │   │   ├── encoder.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── scanner.cpython-311.opt-1.pyc
    │   │       │   │   ├── scanner.cpython-311.opt-2.pyc
    │   │       │   │   ├── scanner.cpython-311.pyc
    │   │       │   │   ├── tool.cpython-311.opt-1.pyc
    │   │       │   │   ├── tool.cpython-311.opt-2.pyc
    │   │       │   │   └── tool.cpython-311.pyc
    │   │       │   ├── scanner.py
    │   │       │   └── tool.py
    │   │       ├── keyword.py
    │   │       ├── lib2to3
    │   │       │   ├── btm_matcher.py
    │   │       │   ├── btm_utils.py
    │   │       │   ├── fixer_base.py
    │   │       │   ├── fixer_util.py
    │   │       │   ├── fixes
    │   │       │   │   ├── fix_apply.py
    │   │       │   │   ├── fix_asserts.py
    │   │       │   │   ├── fix_basestring.py
    │   │       │   │   ├── fix_buffer.py
    │   │       │   │   ├── fix_dict.py
    │   │       │   │   ├── fix_except.py
    │   │       │   │   ├── fix_execfile.py
    │   │       │   │   ├── fix_exec.py
    │   │       │   │   ├── fix_exitfunc.py
    │   │       │   │   ├── fix_filter.py
    │   │       │   │   ├── fix_funcattrs.py
    │   │       │   │   ├── fix_future.py
    │   │       │   │   ├── fix_getcwdu.py
    │   │       │   │   ├── fix_has_key.py
    │   │       │   │   ├── fix_idioms.py
    │   │       │   │   ├── fix_import.py
    │   │       │   │   ├── fix_imports2.py
    │   │       │   │   ├── fix_imports.py
    │   │       │   │   ├── fix_input.py
    │   │       │   │   ├── fix_intern.py
    │   │       │   │   ├── fix_isinstance.py
    │   │       │   │   ├── fix_itertools_imports.py
    │   │       │   │   ├── fix_itertools.py
    │   │       │   │   ├── fix_long.py
    │   │       │   │   ├── fix_map.py
    │   │       │   │   ├── fix_metaclass.py
    │   │       │   │   ├── fix_methodattrs.py
    │   │       │   │   ├── fix_ne.py
    │   │       │   │   ├── fix_next.py
    │   │       │   │   ├── fix_nonzero.py
    │   │       │   │   ├── fix_numliterals.py
    │   │       │   │   ├── fix_operator.py
    │   │       │   │   ├── fix_paren.py
    │   │       │   │   ├── fix_print.py
    │   │       │   │   ├── fix_raise.py
    │   │       │   │   ├── fix_raw_input.py
    │   │       │   │   ├── fix_reduce.py
    │   │       │   │   ├── fix_reload.py
    │   │       │   │   ├── fix_renames.py
    │   │       │   │   ├── fix_repr.py
    │   │       │   │   ├── fix_set_literal.py
    │   │       │   │   ├── fix_standarderror.py
    │   │       │   │   ├── fix_sys_exc.py
    │   │       │   │   ├── fix_throw.py
    │   │       │   │   ├── fix_tuple_params.py
    │   │       │   │   ├── fix_types.py
    │   │       │   │   ├── fix_unicode.py
    │   │       │   │   ├── fix_urllib.py
    │   │       │   │   ├── fix_ws_comma.py
    │   │       │   │   ├── fix_xrange.py
    │   │       │   │   ├── fix_xreadlines.py
    │   │       │   │   ├── fix_zip.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── fix_apply.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_apply.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_apply.cpython-311.pyc
    │   │       │   │       ├── fix_asserts.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_asserts.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_asserts.cpython-311.pyc
    │   │       │   │       ├── fix_basestring.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_basestring.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_basestring.cpython-311.pyc
    │   │       │   │       ├── fix_buffer.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_buffer.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_buffer.cpython-311.pyc
    │   │       │   │       ├── fix_dict.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_dict.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_dict.cpython-311.pyc
    │   │       │   │       ├── fix_except.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_except.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_except.cpython-311.pyc
    │   │       │   │       ├── fix_exec.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_exec.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_exec.cpython-311.pyc
    │   │       │   │       ├── fix_execfile.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_execfile.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_execfile.cpython-311.pyc
    │   │       │   │       ├── fix_exitfunc.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_exitfunc.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_exitfunc.cpython-311.pyc
    │   │       │   │       ├── fix_filter.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_filter.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_filter.cpython-311.pyc
    │   │       │   │       ├── fix_funcattrs.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_funcattrs.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_funcattrs.cpython-311.pyc
    │   │       │   │       ├── fix_future.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_future.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_future.cpython-311.pyc
    │   │       │   │       ├── fix_getcwdu.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_getcwdu.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_getcwdu.cpython-311.pyc
    │   │       │   │       ├── fix_has_key.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_has_key.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_has_key.cpython-311.pyc
    │   │       │   │       ├── fix_idioms.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_idioms.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_idioms.cpython-311.pyc
    │   │       │   │       ├── fix_import.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_import.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_import.cpython-311.pyc
    │   │       │   │       ├── fix_imports2.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_imports2.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_imports2.cpython-311.pyc
    │   │       │   │       ├── fix_imports.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_imports.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_imports.cpython-311.pyc
    │   │       │   │       ├── fix_input.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_input.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_input.cpython-311.pyc
    │   │       │   │       ├── fix_intern.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_intern.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_intern.cpython-311.pyc
    │   │       │   │       ├── fix_isinstance.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_isinstance.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_isinstance.cpython-311.pyc
    │   │       │   │       ├── fix_itertools.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_itertools.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_itertools.cpython-311.pyc
    │   │       │   │       ├── fix_itertools_imports.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_itertools_imports.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_itertools_imports.cpython-311.pyc
    │   │       │   │       ├── fix_long.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_long.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_long.cpython-311.pyc
    │   │       │   │       ├── fix_map.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_map.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_map.cpython-311.pyc
    │   │       │   │       ├── fix_metaclass.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_metaclass.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_metaclass.cpython-311.pyc
    │   │       │   │       ├── fix_methodattrs.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_methodattrs.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_methodattrs.cpython-311.pyc
    │   │       │   │       ├── fix_ne.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_ne.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_ne.cpython-311.pyc
    │   │       │   │       ├── fix_next.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_next.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_next.cpython-311.pyc
    │   │       │   │       ├── fix_nonzero.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_nonzero.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_nonzero.cpython-311.pyc
    │   │       │   │       ├── fix_numliterals.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_numliterals.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_numliterals.cpython-311.pyc
    │   │       │   │       ├── fix_operator.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_operator.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_operator.cpython-311.pyc
    │   │       │   │       ├── fix_paren.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_paren.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_paren.cpython-311.pyc
    │   │       │   │       ├── fix_print.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_print.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_print.cpython-311.pyc
    │   │       │   │       ├── fix_raise.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_raise.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_raise.cpython-311.pyc
    │   │       │   │       ├── fix_raw_input.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_raw_input.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_raw_input.cpython-311.pyc
    │   │       │   │       ├── fix_reduce.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_reduce.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_reduce.cpython-311.pyc
    │   │       │   │       ├── fix_reload.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_reload.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_reload.cpython-311.pyc
    │   │       │   │       ├── fix_renames.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_renames.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_renames.cpython-311.pyc
    │   │       │   │       ├── fix_repr.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_repr.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_repr.cpython-311.pyc
    │   │       │   │       ├── fix_set_literal.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_set_literal.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_set_literal.cpython-311.pyc
    │   │       │   │       ├── fix_standarderror.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_standarderror.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_standarderror.cpython-311.pyc
    │   │       │   │       ├── fix_sys_exc.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_sys_exc.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_sys_exc.cpython-311.pyc
    │   │       │   │       ├── fix_throw.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_throw.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_throw.cpython-311.pyc
    │   │       │   │       ├── fix_tuple_params.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_tuple_params.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_tuple_params.cpython-311.pyc
    │   │       │   │       ├── fix_types.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_types.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_types.cpython-311.pyc
    │   │       │   │       ├── fix_unicode.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_unicode.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_unicode.cpython-311.pyc
    │   │       │   │       ├── fix_urllib.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_urllib.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_urllib.cpython-311.pyc
    │   │       │   │       ├── fix_ws_comma.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_ws_comma.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_ws_comma.cpython-311.pyc
    │   │       │   │       ├── fix_xrange.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_xrange.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_xrange.cpython-311.pyc
    │   │       │   │       ├── fix_xreadlines.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_xreadlines.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_xreadlines.cpython-311.pyc
    │   │       │   │       ├── fix_zip.cpython-311.opt-1.pyc
    │   │       │   │       ├── fix_zip.cpython-311.opt-2.pyc
    │   │       │   │       ├── fix_zip.cpython-311.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   ├── Grammar3.11.4.final.0.pickle
    │   │       │   ├── Grammar.txt
    │   │       │   ├── __init__.py
    │   │       │   ├── __main__.py
    │   │       │   ├── main.py
    │   │       │   ├── patcomp.py
    │   │       │   ├── PatternGrammar3.11.4.final.0.pickle
    │   │       │   ├── PatternGrammar.txt
    │   │       │   ├── pgen2
    │   │       │   │   ├── conv.py
    │   │       │   │   ├── driver.py
    │   │       │   │   ├── grammar.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── literals.py
    │   │       │   │   ├── parse.py
    │   │       │   │   ├── pgen.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── conv.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── conv.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── conv.cpython-311.pyc
    │   │       │   │   │   ├── driver.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── driver.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── driver.cpython-311.pyc
    │   │       │   │   │   ├── grammar.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── grammar.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── grammar.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── literals.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── literals.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── literals.cpython-311.pyc
    │   │       │   │   │   ├── parse.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── parse.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── parse.cpython-311.pyc
    │   │       │   │   │   ├── pgen.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── pgen.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── pgen.cpython-311.pyc
    │   │       │   │   │   ├── token.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── token.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── token.cpython-311.pyc
    │   │       │   │   │   ├── tokenize.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── tokenize.cpython-311.opt-2.pyc
    │   │       │   │   │   └── tokenize.cpython-311.pyc
    │   │       │   │   ├── tokenize.py
    │   │       │   │   └── token.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── btm_matcher.cpython-311.opt-1.pyc
    │   │       │   │   ├── btm_matcher.cpython-311.opt-2.pyc
    │   │       │   │   ├── btm_matcher.cpython-311.pyc
    │   │       │   │   ├── btm_utils.cpython-311.opt-1.pyc
    │   │       │   │   ├── btm_utils.cpython-311.opt-2.pyc
    │   │       │   │   ├── btm_utils.cpython-311.pyc
    │   │       │   │   ├── fixer_base.cpython-311.opt-1.pyc
    │   │       │   │   ├── fixer_base.cpython-311.opt-2.pyc
    │   │       │   │   ├── fixer_base.cpython-311.pyc
    │   │       │   │   ├── fixer_util.cpython-311.opt-1.pyc
    │   │       │   │   ├── fixer_util.cpython-311.opt-2.pyc
    │   │       │   │   ├── fixer_util.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── main.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── main.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── main.cpython-311.pyc
    │   │       │   │   ├── patcomp.cpython-311.opt-1.pyc
    │   │       │   │   ├── patcomp.cpython-311.opt-2.pyc
    │   │       │   │   ├── patcomp.cpython-311.pyc
    │   │       │   │   ├── pygram.cpython-311.opt-1.pyc
    │   │       │   │   ├── pygram.cpython-311.opt-2.pyc
    │   │       │   │   ├── pygram.cpython-311.pyc
    │   │       │   │   ├── pytree.cpython-311.opt-1.pyc
    │   │       │   │   ├── pytree.cpython-311.opt-2.pyc
    │   │       │   │   ├── pytree.cpython-311.pyc
    │   │       │   │   ├── refactor.cpython-311.opt-1.pyc
    │   │       │   │   ├── refactor.cpython-311.opt-2.pyc
    │   │       │   │   └── refactor.cpython-311.pyc
    │   │       │   ├── pygram.py
    │   │       │   ├── pytree.py
    │   │       │   ├── refactor.py
    │   │       │   └── tests
    │   │       │       ├── data
    │   │       │       │   ├── bom.py
    │   │       │       │   ├── crlf.py
    │   │       │       │   ├── different_encoding.py
    │   │       │       │   ├── false_encoding.py
    │   │       │       │   ├── fixers
    │   │       │       │   │   ├── bad_order.py
    │   │       │       │   │   ├── myfixes
    │   │       │       │   │   │   ├── fix_explicit.py
    │   │       │       │   │   │   ├── fix_first.py
    │   │       │       │   │   │   ├── fix_last.py
    │   │       │       │   │   │   ├── fix_parrot.py
    │   │       │       │   │   │   ├── fix_preorder.py
    │   │       │       │   │   │   └── __init__.py
    │   │       │       │   │   ├── no_fixer_cls.py
    │   │       │       │   │   └── parrot_example.py
    │   │       │       │   ├── infinite_recursion.py
    │   │       │       │   ├── py2_test_grammar.py
    │   │       │       │   ├── py3_test_grammar.py
    │   │       │       │   └── README
    │   │       │       ├── __init__.py
    │   │       │       ├── __main__.py
    │   │       │       ├── __pycache__
    │   │       │       │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │       │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │       │   ├── __init__.cpython-311.pyc
    │   │       │       │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │       │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │       │   ├── __main__.cpython-311.pyc
    │   │       │       │   ├── pytree_idempotency.cpython-311.opt-1.pyc
    │   │       │       │   ├── pytree_idempotency.cpython-311.opt-2.pyc
    │   │       │       │   ├── pytree_idempotency.cpython-311.pyc
    │   │       │       │   ├── support.cpython-311.opt-1.pyc
    │   │       │       │   ├── support.cpython-311.opt-2.pyc
    │   │       │       │   ├── support.cpython-311.pyc
    │   │       │       │   ├── test_all_fixers.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_all_fixers.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_all_fixers.cpython-311.pyc
    │   │       │       │   ├── test_fixers.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_fixers.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_fixers.cpython-311.pyc
    │   │       │       │   ├── test_main.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_main.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_main.cpython-311.pyc
    │   │       │       │   ├── test_parser.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_parser.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_parser.cpython-311.pyc
    │   │       │       │   ├── test_pytree.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_pytree.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_pytree.cpython-311.pyc
    │   │       │       │   ├── test_refactor.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_refactor.cpython-311.opt-2.pyc
    │   │       │       │   ├── test_refactor.cpython-311.pyc
    │   │       │       │   ├── test_util.cpython-311.opt-1.pyc
    │   │       │       │   ├── test_util.cpython-311.opt-2.pyc
    │   │       │       │   └── test_util.cpython-311.pyc
    │   │       │       ├── pytree_idempotency.py
    │   │       │       ├── support.py
    │   │       │       ├── test_all_fixers.py
    │   │       │       ├── test_fixers.py
    │   │       │       ├── test_main.py
    │   │       │       ├── test_parser.py
    │   │       │       ├── test_pytree.py
    │   │       │       ├── test_refactor.py
    │   │       │       └── test_util.py
    │   │       ├── lib-dynload
    │   │       │   ├── array.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _asyncio.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── audioop.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── binascii.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _bisect.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _blake2.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _bz2.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── cmath.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_cn.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_hk.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_iso2022.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_jp.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_kr.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _codecs_tw.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _contextvars.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _crypt.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _csv.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _ctypes.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _ctypes_test.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _curses.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _curses_panel.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _datetime.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _decimal.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _elementtree.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── fcntl.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _gdbm.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── grp.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _hashlib.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _heapq.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _json.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _lsprof.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── math.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _md5.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── mmap.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _multibytecodec.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _multiprocessing.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── nis.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _opcode.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── ossaudiodev.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _pickle.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _posixshmem.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _posixsubprocess.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── pyexpat.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _queue.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _random.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── readline.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── resource.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── select.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _sha1.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _sha256.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _sha3.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _sha512.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _socket.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── spwd.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _sqlite3.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _ssl.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _statistics.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _struct.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── syslog.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── termios.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testbuffer.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testcapi.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testclinic.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testimportmultiple.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testinternalcapi.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _testmultiphase.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _typing.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── unicodedata.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── xxlimited_35.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── xxlimited.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _xxsubinterpreters.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── _xxtestfuzz.cpython-311-x86_64-linux-gnu.so
    │   │       │   ├── zlib.cpython-311-x86_64-linux-gnu.so
    │   │       │   └── _zoneinfo.cpython-311-x86_64-linux-gnu.so
    │   │       ├── LICENSE.txt
    │   │       ├── linecache.py
    │   │       ├── locale.py
    │   │       ├── logging
    │   │       │   ├── config.py
    │   │       │   ├── handlers.py
    │   │       │   ├── __init__.py
    │   │       │   └── __pycache__
    │   │       │       ├── config.cpython-311.opt-1.pyc
    │   │       │       ├── config.cpython-311.opt-2.pyc
    │   │       │       ├── config.cpython-311.pyc
    │   │       │       ├── handlers.cpython-311.opt-1.pyc
    │   │       │       ├── handlers.cpython-311.opt-2.pyc
    │   │       │       ├── handlers.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       └── __init__.cpython-311.pyc
    │   │       ├── lzma.py
    │   │       ├── mailbox.py
    │   │       ├── mailcap.py
    │   │       ├── _markupbase.py
    │   │       ├── mimetypes.py
    │   │       ├── modulefinder.py
    │   │       ├── multiprocessing
    │   │       │   ├── connection.py
    │   │       │   ├── context.py
    │   │       │   ├── dummy
    │   │       │   │   ├── connection.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── connection.cpython-311.opt-1.pyc
    │   │       │   │       ├── connection.cpython-311.opt-2.pyc
    │   │       │   │       ├── connection.cpython-311.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   ├── forkserver.py
    │   │       │   ├── heap.py
    │   │       │   ├── __init__.py
    │   │       │   ├── managers.py
    │   │       │   ├── pool.py
    │   │       │   ├── popen_fork.py
    │   │       │   ├── popen_forkserver.py
    │   │       │   ├── popen_spawn_posix.py
    │   │       │   ├── popen_spawn_win32.py
    │   │       │   ├── process.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── connection.cpython-311.opt-1.pyc
    │   │       │   │   ├── connection.cpython-311.opt-2.pyc
    │   │       │   │   ├── connection.cpython-311.pyc
    │   │       │   │   ├── context.cpython-311.opt-1.pyc
    │   │       │   │   ├── context.cpython-311.opt-2.pyc
    │   │       │   │   ├── context.cpython-311.pyc
    │   │       │   │   ├── forkserver.cpython-311.opt-1.pyc
    │   │       │   │   ├── forkserver.cpython-311.opt-2.pyc
    │   │       │   │   ├── forkserver.cpython-311.pyc
    │   │       │   │   ├── heap.cpython-311.opt-1.pyc
    │   │       │   │   ├── heap.cpython-311.opt-2.pyc
    │   │       │   │   ├── heap.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── managers.cpython-311.opt-1.pyc
    │   │       │   │   ├── managers.cpython-311.opt-2.pyc
    │   │       │   │   ├── managers.cpython-311.pyc
    │   │       │   │   ├── pool.cpython-311.opt-1.pyc
    │   │       │   │   ├── pool.cpython-311.opt-2.pyc
    │   │       │   │   ├── pool.cpython-311.pyc
    │   │       │   │   ├── popen_fork.cpython-311.opt-1.pyc
    │   │       │   │   ├── popen_fork.cpython-311.opt-2.pyc
    │   │       │   │   ├── popen_fork.cpython-311.pyc
    │   │       │   │   ├── popen_forkserver.cpython-311.opt-1.pyc
    │   │       │   │   ├── popen_forkserver.cpython-311.opt-2.pyc
    │   │       │   │   ├── popen_forkserver.cpython-311.pyc
    │   │       │   │   ├── popen_spawn_posix.cpython-311.opt-1.pyc
    │   │       │   │   ├── popen_spawn_posix.cpython-311.opt-2.pyc
    │   │       │   │   ├── popen_spawn_posix.cpython-311.pyc
    │   │       │   │   ├── popen_spawn_win32.cpython-311.opt-1.pyc
    │   │       │   │   ├── popen_spawn_win32.cpython-311.opt-2.pyc
    │   │       │   │   ├── popen_spawn_win32.cpython-311.pyc
    │   │       │   │   ├── process.cpython-311.opt-1.pyc
    │   │       │   │   ├── process.cpython-311.opt-2.pyc
    │   │       │   │   ├── process.cpython-311.pyc
    │   │       │   │   ├── queues.cpython-311.opt-1.pyc
    │   │       │   │   ├── queues.cpython-311.opt-2.pyc
    │   │       │   │   ├── queues.cpython-311.pyc
    │   │       │   │   ├── reduction.cpython-311.opt-1.pyc
    │   │       │   │   ├── reduction.cpython-311.opt-2.pyc
    │   │       │   │   ├── reduction.cpython-311.pyc
    │   │       │   │   ├── resource_sharer.cpython-311.opt-1.pyc
    │   │       │   │   ├── resource_sharer.cpython-311.opt-2.pyc
    │   │       │   │   ├── resource_sharer.cpython-311.pyc
    │   │       │   │   ├── resource_tracker.cpython-311.opt-1.pyc
    │   │       │   │   ├── resource_tracker.cpython-311.opt-2.pyc
    │   │       │   │   ├── resource_tracker.cpython-311.pyc
    │   │       │   │   ├── sharedctypes.cpython-311.opt-1.pyc
    │   │       │   │   ├── sharedctypes.cpython-311.opt-2.pyc
    │   │       │   │   ├── sharedctypes.cpython-311.pyc
    │   │       │   │   ├── shared_memory.cpython-311.opt-1.pyc
    │   │       │   │   ├── shared_memory.cpython-311.opt-2.pyc
    │   │       │   │   ├── shared_memory.cpython-311.pyc
    │   │       │   │   ├── spawn.cpython-311.opt-1.pyc
    │   │       │   │   ├── spawn.cpython-311.opt-2.pyc
    │   │       │   │   ├── spawn.cpython-311.pyc
    │   │       │   │   ├── synchronize.cpython-311.opt-1.pyc
    │   │       │   │   ├── synchronize.cpython-311.opt-2.pyc
    │   │       │   │   ├── synchronize.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   └── util.cpython-311.pyc
    │   │       │   ├── queues.py
    │   │       │   ├── reduction.py
    │   │       │   ├── resource_sharer.py
    │   │       │   ├── resource_tracker.py
    │   │       │   ├── sharedctypes.py
    │   │       │   ├── shared_memory.py
    │   │       │   ├── spawn.py
    │   │       │   ├── synchronize.py
    │   │       │   └── util.py
    │   │       ├── netrc.py
    │   │       ├── nntplib.py
    │   │       ├── ntpath.py
    │   │       ├── nturl2path.py
    │   │       ├── numbers.py
    │   │       ├── opcode.py
    │   │       ├── operator.py
    │   │       ├── optparse.py
    │   │       ├── os.py
    │   │       ├── _osx_support.py
    │   │       ├── pathlib.py
    │   │       ├── pdb.py
    │   │       ├── __phello__
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── spam.cpython-311.opt-1.pyc
    │   │       │   │   ├── spam.cpython-311.opt-2.pyc
    │   │       │   │   └── spam.cpython-311.pyc
    │   │       │   └── spam.py
    │   │       ├── pickle.py
    │   │       ├── pickletools.py
    │   │       ├── pipes.py
    │   │       ├── pkgutil.py
    │   │       ├── platform.py
    │   │       ├── plistlib.py
    │   │       ├── poplib.py
    │   │       ├── posixpath.py
    │   │       ├── pprint.py
    │   │       ├── profile.py
    │   │       ├── pstats.py
    │   │       ├── pty.py
    │   │       ├── _py_abc.py
    │   │       ├── __pycache__
    │   │       │   ├── abc.cpython-311.opt-1.pyc
    │   │       │   ├── abc.cpython-311.opt-2.pyc
    │   │       │   ├── abc.cpython-311.pyc
    │   │       │   ├── aifc.cpython-311.opt-1.pyc
    │   │       │   ├── aifc.cpython-311.opt-2.pyc
    │   │       │   ├── aifc.cpython-311.pyc
    │   │       │   ├── _aix_support.cpython-311.opt-1.pyc
    │   │       │   ├── _aix_support.cpython-311.opt-2.pyc
    │   │       │   ├── _aix_support.cpython-311.pyc
    │   │       │   ├── antigravity.cpython-311.opt-1.pyc
    │   │       │   ├── antigravity.cpython-311.opt-2.pyc
    │   │       │   ├── antigravity.cpython-311.pyc
    │   │       │   ├── argparse.cpython-311.opt-1.pyc
    │   │       │   ├── argparse.cpython-311.opt-2.pyc
    │   │       │   ├── argparse.cpython-311.pyc
    │   │       │   ├── ast.cpython-311.opt-1.pyc
    │   │       │   ├── ast.cpython-311.opt-2.pyc
    │   │       │   ├── ast.cpython-311.pyc
    │   │       │   ├── asynchat.cpython-311.opt-1.pyc
    │   │       │   ├── asynchat.cpython-311.opt-2.pyc
    │   │       │   ├── asynchat.cpython-311.pyc
    │   │       │   ├── asyncore.cpython-311.opt-1.pyc
    │   │       │   ├── asyncore.cpython-311.opt-2.pyc
    │   │       │   ├── asyncore.cpython-311.pyc
    │   │       │   ├── base64.cpython-311.opt-1.pyc
    │   │       │   ├── base64.cpython-311.opt-2.pyc
    │   │       │   ├── base64.cpython-311.pyc
    │   │       │   ├── bdb.cpython-311.opt-1.pyc
    │   │       │   ├── bdb.cpython-311.opt-2.pyc
    │   │       │   ├── bdb.cpython-311.pyc
    │   │       │   ├── bisect.cpython-311.opt-1.pyc
    │   │       │   ├── bisect.cpython-311.opt-2.pyc
    │   │       │   ├── bisect.cpython-311.pyc
    │   │       │   ├── _bootsubprocess.cpython-311.opt-1.pyc
    │   │       │   ├── _bootsubprocess.cpython-311.opt-2.pyc
    │   │       │   ├── _bootsubprocess.cpython-311.pyc
    │   │       │   ├── bz2.cpython-311.opt-1.pyc
    │   │       │   ├── bz2.cpython-311.opt-2.pyc
    │   │       │   ├── bz2.cpython-311.pyc
    │   │       │   ├── calendar.cpython-311.opt-1.pyc
    │   │       │   ├── calendar.cpython-311.opt-2.pyc
    │   │       │   ├── calendar.cpython-311.pyc
    │   │       │   ├── cgi.cpython-311.opt-1.pyc
    │   │       │   ├── cgi.cpython-311.opt-2.pyc
    │   │       │   ├── cgi.cpython-311.pyc
    │   │       │   ├── cgitb.cpython-311.opt-1.pyc
    │   │       │   ├── cgitb.cpython-311.opt-2.pyc
    │   │       │   ├── cgitb.cpython-311.pyc
    │   │       │   ├── chunk.cpython-311.opt-1.pyc
    │   │       │   ├── chunk.cpython-311.opt-2.pyc
    │   │       │   ├── chunk.cpython-311.pyc
    │   │       │   ├── cmd.cpython-311.opt-1.pyc
    │   │       │   ├── cmd.cpython-311.opt-2.pyc
    │   │       │   ├── cmd.cpython-311.pyc
    │   │       │   ├── code.cpython-311.opt-1.pyc
    │   │       │   ├── code.cpython-311.opt-2.pyc
    │   │       │   ├── code.cpython-311.pyc
    │   │       │   ├── codecs.cpython-311.opt-1.pyc
    │   │       │   ├── codecs.cpython-311.opt-2.pyc
    │   │       │   ├── codecs.cpython-311.pyc
    │   │       │   ├── codeop.cpython-311.opt-1.pyc
    │   │       │   ├── codeop.cpython-311.opt-2.pyc
    │   │       │   ├── codeop.cpython-311.pyc
    │   │       │   ├── _collections_abc.cpython-311.opt-1.pyc
    │   │       │   ├── _collections_abc.cpython-311.opt-2.pyc
    │   │       │   ├── _collections_abc.cpython-311.pyc
    │   │       │   ├── colorsys.cpython-311.opt-1.pyc
    │   │       │   ├── colorsys.cpython-311.opt-2.pyc
    │   │       │   ├── colorsys.cpython-311.pyc
    │   │       │   ├── _compat_pickle.cpython-311.opt-1.pyc
    │   │       │   ├── _compat_pickle.cpython-311.opt-2.pyc
    │   │       │   ├── _compat_pickle.cpython-311.pyc
    │   │       │   ├── compileall.cpython-311.opt-1.pyc
    │   │       │   ├── compileall.cpython-311.opt-2.pyc
    │   │       │   ├── compileall.cpython-311.pyc
    │   │       │   ├── _compression.cpython-311.opt-1.pyc
    │   │       │   ├── _compression.cpython-311.opt-2.pyc
    │   │       │   ├── _compression.cpython-311.pyc
    │   │       │   ├── configparser.cpython-311.opt-1.pyc
    │   │       │   ├── configparser.cpython-311.opt-2.pyc
    │   │       │   ├── configparser.cpython-311.pyc
    │   │       │   ├── contextlib.cpython-311.opt-1.pyc
    │   │       │   ├── contextlib.cpython-311.opt-2.pyc
    │   │       │   ├── contextlib.cpython-311.pyc
    │   │       │   ├── contextvars.cpython-311.opt-1.pyc
    │   │       │   ├── contextvars.cpython-311.opt-2.pyc
    │   │       │   ├── contextvars.cpython-311.pyc
    │   │       │   ├── copy.cpython-311.opt-1.pyc
    │   │       │   ├── copy.cpython-311.opt-2.pyc
    │   │       │   ├── copy.cpython-311.pyc
    │   │       │   ├── copyreg.cpython-311.opt-1.pyc
    │   │       │   ├── copyreg.cpython-311.opt-2.pyc
    │   │       │   ├── copyreg.cpython-311.pyc
    │   │       │   ├── cProfile.cpython-311.opt-1.pyc
    │   │       │   ├── cProfile.cpython-311.opt-2.pyc
    │   │       │   ├── cProfile.cpython-311.pyc
    │   │       │   ├── crypt.cpython-311.opt-1.pyc
    │   │       │   ├── crypt.cpython-311.opt-2.pyc
    │   │       │   ├── crypt.cpython-311.pyc
    │   │       │   ├── csv.cpython-311.opt-1.pyc
    │   │       │   ├── csv.cpython-311.opt-2.pyc
    │   │       │   ├── csv.cpython-311.pyc
    │   │       │   ├── dataclasses.cpython-311.opt-1.pyc
    │   │       │   ├── dataclasses.cpython-311.opt-2.pyc
    │   │       │   ├── dataclasses.cpython-311.pyc
    │   │       │   ├── datetime.cpython-311.opt-1.pyc
    │   │       │   ├── datetime.cpython-311.opt-2.pyc
    │   │       │   ├── datetime.cpython-311.pyc
    │   │       │   ├── decimal.cpython-311.opt-1.pyc
    │   │       │   ├── decimal.cpython-311.opt-2.pyc
    │   │       │   ├── decimal.cpython-311.pyc
    │   │       │   ├── difflib.cpython-311.opt-1.pyc
    │   │       │   ├── difflib.cpython-311.opt-2.pyc
    │   │       │   ├── difflib.cpython-311.pyc
    │   │       │   ├── dis.cpython-311.opt-1.pyc
    │   │       │   ├── dis.cpython-311.opt-2.pyc
    │   │       │   ├── dis.cpython-311.pyc
    │   │       │   ├── doctest.cpython-311.opt-1.pyc
    │   │       │   ├── doctest.cpython-311.opt-2.pyc
    │   │       │   ├── doctest.cpython-311.pyc
    │   │       │   ├── enum.cpython-311.opt-1.pyc
    │   │       │   ├── enum.cpython-311.opt-2.pyc
    │   │       │   ├── enum.cpython-311.pyc
    │   │       │   ├── filecmp.cpython-311.opt-1.pyc
    │   │       │   ├── filecmp.cpython-311.opt-2.pyc
    │   │       │   ├── filecmp.cpython-311.pyc
    │   │       │   ├── fileinput.cpython-311.opt-1.pyc
    │   │       │   ├── fileinput.cpython-311.opt-2.pyc
    │   │       │   ├── fileinput.cpython-311.pyc
    │   │       │   ├── fnmatch.cpython-311.opt-1.pyc
    │   │       │   ├── fnmatch.cpython-311.opt-2.pyc
    │   │       │   ├── fnmatch.cpython-311.pyc
    │   │       │   ├── fractions.cpython-311.opt-1.pyc
    │   │       │   ├── fractions.cpython-311.opt-2.pyc
    │   │       │   ├── fractions.cpython-311.pyc
    │   │       │   ├── ftplib.cpython-311.opt-1.pyc
    │   │       │   ├── ftplib.cpython-311.opt-2.pyc
    │   │       │   ├── ftplib.cpython-311.pyc
    │   │       │   ├── functools.cpython-311.opt-1.pyc
    │   │       │   ├── functools.cpython-311.opt-2.pyc
    │   │       │   ├── functools.cpython-311.pyc
    │   │       │   ├── __future__.cpython-311.opt-1.pyc
    │   │       │   ├── __future__.cpython-311.opt-2.pyc
    │   │       │   ├── __future__.cpython-311.pyc
    │   │       │   ├── genericpath.cpython-311.opt-1.pyc
    │   │       │   ├── genericpath.cpython-311.opt-2.pyc
    │   │       │   ├── genericpath.cpython-311.pyc
    │   │       │   ├── getopt.cpython-311.opt-1.pyc
    │   │       │   ├── getopt.cpython-311.opt-2.pyc
    │   │       │   ├── getopt.cpython-311.pyc
    │   │       │   ├── getpass.cpython-311.opt-1.pyc
    │   │       │   ├── getpass.cpython-311.opt-2.pyc
    │   │       │   ├── getpass.cpython-311.pyc
    │   │       │   ├── gettext.cpython-311.opt-1.pyc
    │   │       │   ├── gettext.cpython-311.opt-2.pyc
    │   │       │   ├── gettext.cpython-311.pyc
    │   │       │   ├── glob.cpython-311.opt-1.pyc
    │   │       │   ├── glob.cpython-311.opt-2.pyc
    │   │       │   ├── glob.cpython-311.pyc
    │   │       │   ├── graphlib.cpython-311.opt-1.pyc
    │   │       │   ├── graphlib.cpython-311.opt-2.pyc
    │   │       │   ├── graphlib.cpython-311.pyc
    │   │       │   ├── gzip.cpython-311.opt-1.pyc
    │   │       │   ├── gzip.cpython-311.opt-2.pyc
    │   │       │   ├── gzip.cpython-311.pyc
    │   │       │   ├── hashlib.cpython-311.opt-1.pyc
    │   │       │   ├── hashlib.cpython-311.opt-2.pyc
    │   │       │   ├── hashlib.cpython-311.pyc
    │   │       │   ├── heapq.cpython-311.opt-1.pyc
    │   │       │   ├── heapq.cpython-311.opt-2.pyc
    │   │       │   ├── heapq.cpython-311.pyc
    │   │       │   ├── __hello__.cpython-311.opt-1.pyc
    │   │       │   ├── __hello__.cpython-311.opt-2.pyc
    │   │       │   ├── __hello__.cpython-311.pyc
    │   │       │   ├── hmac.cpython-311.opt-1.pyc
    │   │       │   ├── hmac.cpython-311.opt-2.pyc
    │   │       │   ├── hmac.cpython-311.pyc
    │   │       │   ├── imaplib.cpython-311.opt-1.pyc
    │   │       │   ├── imaplib.cpython-311.opt-2.pyc
    │   │       │   ├── imaplib.cpython-311.pyc
    │   │       │   ├── imghdr.cpython-311.opt-1.pyc
    │   │       │   ├── imghdr.cpython-311.opt-2.pyc
    │   │       │   ├── imghdr.cpython-311.pyc
    │   │       │   ├── imp.cpython-311.opt-1.pyc
    │   │       │   ├── imp.cpython-311.opt-2.pyc
    │   │       │   ├── imp.cpython-311.pyc
    │   │       │   ├── inspect.cpython-311.opt-1.pyc
    │   │       │   ├── inspect.cpython-311.opt-2.pyc
    │   │       │   ├── inspect.cpython-311.pyc
    │   │       │   ├── io.cpython-311.opt-1.pyc
    │   │       │   ├── io.cpython-311.opt-2.pyc
    │   │       │   ├── io.cpython-311.pyc
    │   │       │   ├── ipaddress.cpython-311.opt-1.pyc
    │   │       │   ├── ipaddress.cpython-311.opt-2.pyc
    │   │       │   ├── ipaddress.cpython-311.pyc
    │   │       │   ├── keyword.cpython-311.opt-1.pyc
    │   │       │   ├── keyword.cpython-311.opt-2.pyc
    │   │       │   ├── keyword.cpython-311.pyc
    │   │       │   ├── linecache.cpython-311.opt-1.pyc
    │   │       │   ├── linecache.cpython-311.opt-2.pyc
    │   │       │   ├── linecache.cpython-311.pyc
    │   │       │   ├── locale.cpython-311.opt-1.pyc
    │   │       │   ├── locale.cpython-311.opt-2.pyc
    │   │       │   ├── locale.cpython-311.pyc
    │   │       │   ├── lzma.cpython-311.opt-1.pyc
    │   │       │   ├── lzma.cpython-311.opt-2.pyc
    │   │       │   ├── lzma.cpython-311.pyc
    │   │       │   ├── mailbox.cpython-311.opt-1.pyc
    │   │       │   ├── mailbox.cpython-311.opt-2.pyc
    │   │       │   ├── mailbox.cpython-311.pyc
    │   │       │   ├── mailcap.cpython-311.opt-1.pyc
    │   │       │   ├── mailcap.cpython-311.opt-2.pyc
    │   │       │   ├── mailcap.cpython-311.pyc
    │   │       │   ├── _markupbase.cpython-311.opt-1.pyc
    │   │       │   ├── _markupbase.cpython-311.opt-2.pyc
    │   │       │   ├── _markupbase.cpython-311.pyc
    │   │       │   ├── mimetypes.cpython-311.opt-1.pyc
    │   │       │   ├── mimetypes.cpython-311.opt-2.pyc
    │   │       │   ├── mimetypes.cpython-311.pyc
    │   │       │   ├── modulefinder.cpython-311.opt-1.pyc
    │   │       │   ├── modulefinder.cpython-311.opt-2.pyc
    │   │       │   ├── modulefinder.cpython-311.pyc
    │   │       │   ├── netrc.cpython-311.opt-1.pyc
    │   │       │   ├── netrc.cpython-311.opt-2.pyc
    │   │       │   ├── netrc.cpython-311.pyc
    │   │       │   ├── nntplib.cpython-311.opt-1.pyc
    │   │       │   ├── nntplib.cpython-311.opt-2.pyc
    │   │       │   ├── nntplib.cpython-311.pyc
    │   │       │   ├── ntpath.cpython-311.opt-1.pyc
    │   │       │   ├── ntpath.cpython-311.opt-2.pyc
    │   │       │   ├── ntpath.cpython-311.pyc
    │   │       │   ├── nturl2path.cpython-311.opt-1.pyc
    │   │       │   ├── nturl2path.cpython-311.opt-2.pyc
    │   │       │   ├── nturl2path.cpython-311.pyc
    │   │       │   ├── numbers.cpython-311.opt-1.pyc
    │   │       │   ├── numbers.cpython-311.opt-2.pyc
    │   │       │   ├── numbers.cpython-311.pyc
    │   │       │   ├── opcode.cpython-311.opt-1.pyc
    │   │       │   ├── opcode.cpython-311.opt-2.pyc
    │   │       │   ├── opcode.cpython-311.pyc
    │   │       │   ├── operator.cpython-311.opt-1.pyc
    │   │       │   ├── operator.cpython-311.opt-2.pyc
    │   │       │   ├── operator.cpython-311.pyc
    │   │       │   ├── optparse.cpython-311.opt-1.pyc
    │   │       │   ├── optparse.cpython-311.opt-2.pyc
    │   │       │   ├── optparse.cpython-311.pyc
    │   │       │   ├── os.cpython-311.opt-1.pyc
    │   │       │   ├── os.cpython-311.opt-2.pyc
    │   │       │   ├── os.cpython-311.pyc
    │   │       │   ├── _osx_support.cpython-311.opt-1.pyc
    │   │       │   ├── _osx_support.cpython-311.opt-2.pyc
    │   │       │   ├── _osx_support.cpython-311.pyc
    │   │       │   ├── pathlib.cpython-311.opt-1.pyc
    │   │       │   ├── pathlib.cpython-311.opt-2.pyc
    │   │       │   ├── pathlib.cpython-311.pyc
    │   │       │   ├── pdb.cpython-311.opt-1.pyc
    │   │       │   ├── pdb.cpython-311.opt-2.pyc
    │   │       │   ├── pdb.cpython-311.pyc
    │   │       │   ├── pickle.cpython-311.opt-1.pyc
    │   │       │   ├── pickle.cpython-311.opt-2.pyc
    │   │       │   ├── pickle.cpython-311.pyc
    │   │       │   ├── pickletools.cpython-311.opt-1.pyc
    │   │       │   ├── pickletools.cpython-311.opt-2.pyc
    │   │       │   ├── pickletools.cpython-311.pyc
    │   │       │   ├── pipes.cpython-311.opt-1.pyc
    │   │       │   ├── pipes.cpython-311.opt-2.pyc
    │   │       │   ├── pipes.cpython-311.pyc
    │   │       │   ├── pkgutil.cpython-311.opt-1.pyc
    │   │       │   ├── pkgutil.cpython-311.opt-2.pyc
    │   │       │   ├── pkgutil.cpython-311.pyc
    │   │       │   ├── platform.cpython-311.opt-1.pyc
    │   │       │   ├── platform.cpython-311.opt-2.pyc
    │   │       │   ├── platform.cpython-311.pyc
    │   │       │   ├── plistlib.cpython-311.opt-1.pyc
    │   │       │   ├── plistlib.cpython-311.opt-2.pyc
    │   │       │   ├── plistlib.cpython-311.pyc
    │   │       │   ├── poplib.cpython-311.opt-1.pyc
    │   │       │   ├── poplib.cpython-311.opt-2.pyc
    │   │       │   ├── poplib.cpython-311.pyc
    │   │       │   ├── posixpath.cpython-311.opt-1.pyc
    │   │       │   ├── posixpath.cpython-311.opt-2.pyc
    │   │       │   ├── posixpath.cpython-311.pyc
    │   │       │   ├── pprint.cpython-311.opt-1.pyc
    │   │       │   ├── pprint.cpython-311.opt-2.pyc
    │   │       │   ├── pprint.cpython-311.pyc
    │   │       │   ├── profile.cpython-311.opt-1.pyc
    │   │       │   ├── profile.cpython-311.opt-2.pyc
    │   │       │   ├── profile.cpython-311.pyc
    │   │       │   ├── pstats.cpython-311.opt-1.pyc
    │   │       │   ├── pstats.cpython-311.opt-2.pyc
    │   │       │   ├── pstats.cpython-311.pyc
    │   │       │   ├── pty.cpython-311.opt-1.pyc
    │   │       │   ├── pty.cpython-311.opt-2.pyc
    │   │       │   ├── pty.cpython-311.pyc
    │   │       │   ├── _py_abc.cpython-311.opt-1.pyc
    │   │       │   ├── _py_abc.cpython-311.opt-2.pyc
    │   │       │   ├── _py_abc.cpython-311.pyc
    │   │       │   ├── pyclbr.cpython-311.opt-1.pyc
    │   │       │   ├── pyclbr.cpython-311.opt-2.pyc
    │   │       │   ├── pyclbr.cpython-311.pyc
    │   │       │   ├── py_compile.cpython-311.opt-1.pyc
    │   │       │   ├── py_compile.cpython-311.opt-2.pyc
    │   │       │   ├── py_compile.cpython-311.pyc
    │   │       │   ├── _pydecimal.cpython-311.opt-1.pyc
    │   │       │   ├── _pydecimal.cpython-311.opt-2.pyc
    │   │       │   ├── _pydecimal.cpython-311.pyc
    │   │       │   ├── pydoc.cpython-311.opt-1.pyc
    │   │       │   ├── pydoc.cpython-311.opt-2.pyc
    │   │       │   ├── pydoc.cpython-311.pyc
    │   │       │   ├── _pyio.cpython-311.opt-1.pyc
    │   │       │   ├── _pyio.cpython-311.opt-2.pyc
    │   │       │   ├── _pyio.cpython-311.pyc
    │   │       │   ├── queue.cpython-311.opt-1.pyc
    │   │       │   ├── queue.cpython-311.opt-2.pyc
    │   │       │   ├── queue.cpython-311.pyc
    │   │       │   ├── quopri.cpython-311.opt-1.pyc
    │   │       │   ├── quopri.cpython-311.opt-2.pyc
    │   │       │   ├── quopri.cpython-311.pyc
    │   │       │   ├── random.cpython-311.opt-1.pyc
    │   │       │   ├── random.cpython-311.opt-2.pyc
    │   │       │   ├── random.cpython-311.pyc
    │   │       │   ├── reprlib.cpython-311.opt-1.pyc
    │   │       │   ├── reprlib.cpython-311.opt-2.pyc
    │   │       │   ├── reprlib.cpython-311.pyc
    │   │       │   ├── rlcompleter.cpython-311.opt-1.pyc
    │   │       │   ├── rlcompleter.cpython-311.opt-2.pyc
    │   │       │   ├── rlcompleter.cpython-311.pyc
    │   │       │   ├── runpy.cpython-311.opt-1.pyc
    │   │       │   ├── runpy.cpython-311.opt-2.pyc
    │   │       │   ├── runpy.cpython-311.pyc
    │   │       │   ├── sched.cpython-311.opt-1.pyc
    │   │       │   ├── sched.cpython-311.opt-2.pyc
    │   │       │   ├── sched.cpython-311.pyc
    │   │       │   ├── secrets.cpython-311.opt-1.pyc
    │   │       │   ├── secrets.cpython-311.opt-2.pyc
    │   │       │   ├── secrets.cpython-311.pyc
    │   │       │   ├── selectors.cpython-311.opt-1.pyc
    │   │       │   ├── selectors.cpython-311.opt-2.pyc
    │   │       │   ├── selectors.cpython-311.pyc
    │   │       │   ├── shelve.cpython-311.opt-1.pyc
    │   │       │   ├── shelve.cpython-311.opt-2.pyc
    │   │       │   ├── shelve.cpython-311.pyc
    │   │       │   ├── shlex.cpython-311.opt-1.pyc
    │   │       │   ├── shlex.cpython-311.opt-2.pyc
    │   │       │   ├── shlex.cpython-311.pyc
    │   │       │   ├── shutil.cpython-311.opt-1.pyc
    │   │       │   ├── shutil.cpython-311.opt-2.pyc
    │   │       │   ├── shutil.cpython-311.pyc
    │   │       │   ├── signal.cpython-311.opt-1.pyc
    │   │       │   ├── signal.cpython-311.opt-2.pyc
    │   │       │   ├── signal.cpython-311.pyc
    │   │       │   ├── _sitebuiltins.cpython-311.opt-1.pyc
    │   │       │   ├── _sitebuiltins.cpython-311.opt-2.pyc
    │   │       │   ├── _sitebuiltins.cpython-311.pyc
    │   │       │   ├── site.cpython-311.opt-1.pyc
    │   │       │   ├── site.cpython-311.opt-2.pyc
    │   │       │   ├── site.cpython-311.pyc
    │   │       │   ├── smtpd.cpython-311.opt-1.pyc
    │   │       │   ├── smtpd.cpython-311.opt-2.pyc
    │   │       │   ├── smtpd.cpython-311.pyc
    │   │       │   ├── smtplib.cpython-311.opt-1.pyc
    │   │       │   ├── smtplib.cpython-311.opt-2.pyc
    │   │       │   ├── smtplib.cpython-311.pyc
    │   │       │   ├── sndhdr.cpython-311.opt-1.pyc
    │   │       │   ├── sndhdr.cpython-311.opt-2.pyc
    │   │       │   ├── sndhdr.cpython-311.pyc
    │   │       │   ├── socket.cpython-311.opt-1.pyc
    │   │       │   ├── socket.cpython-311.opt-2.pyc
    │   │       │   ├── socket.cpython-311.pyc
    │   │       │   ├── socketserver.cpython-311.opt-1.pyc
    │   │       │   ├── socketserver.cpython-311.opt-2.pyc
    │   │       │   ├── socketserver.cpython-311.pyc
    │   │       │   ├── sre_compile.cpython-311.opt-1.pyc
    │   │       │   ├── sre_compile.cpython-311.opt-2.pyc
    │   │       │   ├── sre_compile.cpython-311.pyc
    │   │       │   ├── sre_constants.cpython-311.opt-1.pyc
    │   │       │   ├── sre_constants.cpython-311.opt-2.pyc
    │   │       │   ├── sre_constants.cpython-311.pyc
    │   │       │   ├── sre_parse.cpython-311.opt-1.pyc
    │   │       │   ├── sre_parse.cpython-311.opt-2.pyc
    │   │       │   ├── sre_parse.cpython-311.pyc
    │   │       │   ├── ssl.cpython-311.opt-1.pyc
    │   │       │   ├── ssl.cpython-311.opt-2.pyc
    │   │       │   ├── ssl.cpython-311.pyc
    │   │       │   ├── stat.cpython-311.opt-1.pyc
    │   │       │   ├── stat.cpython-311.opt-2.pyc
    │   │       │   ├── stat.cpython-311.pyc
    │   │       │   ├── statistics.cpython-311.opt-1.pyc
    │   │       │   ├── statistics.cpython-311.opt-2.pyc
    │   │       │   ├── statistics.cpython-311.pyc
    │   │       │   ├── string.cpython-311.opt-1.pyc
    │   │       │   ├── string.cpython-311.opt-2.pyc
    │   │       │   ├── string.cpython-311.pyc
    │   │       │   ├── stringprep.cpython-311.opt-1.pyc
    │   │       │   ├── stringprep.cpython-311.opt-2.pyc
    │   │       │   ├── stringprep.cpython-311.pyc
    │   │       │   ├── _strptime.cpython-311.opt-1.pyc
    │   │       │   ├── _strptime.cpython-311.opt-2.pyc
    │   │       │   ├── _strptime.cpython-311.pyc
    │   │       │   ├── struct.cpython-311.opt-1.pyc
    │   │       │   ├── struct.cpython-311.opt-2.pyc
    │   │       │   ├── struct.cpython-311.pyc
    │   │       │   ├── subprocess.cpython-311.opt-1.pyc
    │   │       │   ├── subprocess.cpython-311.opt-2.pyc
    │   │       │   ├── subprocess.cpython-311.pyc
    │   │       │   ├── sunau.cpython-311.opt-1.pyc
    │   │       │   ├── sunau.cpython-311.opt-2.pyc
    │   │       │   ├── sunau.cpython-311.pyc
    │   │       │   ├── symtable.cpython-311.opt-1.pyc
    │   │       │   ├── symtable.cpython-311.opt-2.pyc
    │   │       │   ├── symtable.cpython-311.pyc
    │   │       │   ├── sysconfig.cpython-311.opt-1.pyc
    │   │       │   ├── sysconfig.cpython-311.opt-2.pyc
    │   │       │   ├── sysconfig.cpython-311.pyc
    │   │       │   ├── _sysconfigdata__linux_x86_64-linux-gnu.cpython-311.opt-1.pyc
    │   │       │   ├── _sysconfigdata__linux_x86_64-linux-gnu.cpython-311.opt-2.pyc
    │   │       │   ├── _sysconfigdata__linux_x86_64-linux-gnu.cpython-311.pyc
    │   │       │   ├── tabnanny.cpython-311.opt-1.pyc
    │   │       │   ├── tabnanny.cpython-311.opt-2.pyc
    │   │       │   ├── tabnanny.cpython-311.pyc
    │   │       │   ├── tarfile.cpython-311.opt-1.pyc
    │   │       │   ├── tarfile.cpython-311.opt-2.pyc
    │   │       │   ├── tarfile.cpython-311.pyc
    │   │       │   ├── telnetlib.cpython-311.opt-1.pyc
    │   │       │   ├── telnetlib.cpython-311.opt-2.pyc
    │   │       │   ├── telnetlib.cpython-311.pyc
    │   │       │   ├── tempfile.cpython-311.opt-1.pyc
    │   │       │   ├── tempfile.cpython-311.opt-2.pyc
    │   │       │   ├── tempfile.cpython-311.pyc
    │   │       │   ├── textwrap.cpython-311.opt-1.pyc
    │   │       │   ├── textwrap.cpython-311.opt-2.pyc
    │   │       │   ├── textwrap.cpython-311.pyc
    │   │       │   ├── this.cpython-311.opt-1.pyc
    │   │       │   ├── this.cpython-311.opt-2.pyc
    │   │       │   ├── this.cpython-311.pyc
    │   │       │   ├── threading.cpython-311.opt-1.pyc
    │   │       │   ├── threading.cpython-311.opt-2.pyc
    │   │       │   ├── threading.cpython-311.pyc
    │   │       │   ├── _threading_local.cpython-311.opt-1.pyc
    │   │       │   ├── _threading_local.cpython-311.opt-2.pyc
    │   │       │   ├── _threading_local.cpython-311.pyc
    │   │       │   ├── timeit.cpython-311.opt-1.pyc
    │   │       │   ├── timeit.cpython-311.opt-2.pyc
    │   │       │   ├── timeit.cpython-311.pyc
    │   │       │   ├── token.cpython-311.opt-1.pyc
    │   │       │   ├── token.cpython-311.opt-2.pyc
    │   │       │   ├── token.cpython-311.pyc
    │   │       │   ├── tokenize.cpython-311.opt-1.pyc
    │   │       │   ├── tokenize.cpython-311.opt-2.pyc
    │   │       │   ├── tokenize.cpython-311.pyc
    │   │       │   ├── traceback.cpython-311.opt-1.pyc
    │   │       │   ├── traceback.cpython-311.opt-2.pyc
    │   │       │   ├── traceback.cpython-311.pyc
    │   │       │   ├── trace.cpython-311.opt-1.pyc
    │   │       │   ├── trace.cpython-311.opt-2.pyc
    │   │       │   ├── trace.cpython-311.pyc
    │   │       │   ├── tracemalloc.cpython-311.opt-1.pyc
    │   │       │   ├── tracemalloc.cpython-311.opt-2.pyc
    │   │       │   ├── tracemalloc.cpython-311.pyc
    │   │       │   ├── tty.cpython-311.opt-1.pyc
    │   │       │   ├── tty.cpython-311.opt-2.pyc
    │   │       │   ├── tty.cpython-311.pyc
    │   │       │   ├── turtle.cpython-311.opt-1.pyc
    │   │       │   ├── turtle.cpython-311.opt-2.pyc
    │   │       │   ├── turtle.cpython-311.pyc
    │   │       │   ├── types.cpython-311.opt-1.pyc
    │   │       │   ├── types.cpython-311.opt-2.pyc
    │   │       │   ├── types.cpython-311.pyc
    │   │       │   ├── typing.cpython-311.opt-1.pyc
    │   │       │   ├── typing.cpython-311.opt-2.pyc
    │   │       │   ├── typing.cpython-311.pyc
    │   │       │   ├── uu.cpython-311.opt-1.pyc
    │   │       │   ├── uu.cpython-311.opt-2.pyc
    │   │       │   ├── uu.cpython-311.pyc
    │   │       │   ├── uuid.cpython-311.opt-1.pyc
    │   │       │   ├── uuid.cpython-311.opt-2.pyc
    │   │       │   ├── uuid.cpython-311.pyc
    │   │       │   ├── warnings.cpython-311.opt-1.pyc
    │   │       │   ├── warnings.cpython-311.opt-2.pyc
    │   │       │   ├── warnings.cpython-311.pyc
    │   │       │   ├── wave.cpython-311.opt-1.pyc
    │   │       │   ├── wave.cpython-311.opt-2.pyc
    │   │       │   ├── wave.cpython-311.pyc
    │   │       │   ├── weakref.cpython-311.opt-1.pyc
    │   │       │   ├── weakref.cpython-311.opt-2.pyc
    │   │       │   ├── weakref.cpython-311.pyc
    │   │       │   ├── _weakrefset.cpython-311.opt-1.pyc
    │   │       │   ├── _weakrefset.cpython-311.opt-2.pyc
    │   │       │   ├── _weakrefset.cpython-311.pyc
    │   │       │   ├── webbrowser.cpython-311.opt-1.pyc
    │   │       │   ├── webbrowser.cpython-311.opt-2.pyc
    │   │       │   ├── webbrowser.cpython-311.pyc
    │   │       │   ├── xdrlib.cpython-311.opt-1.pyc
    │   │       │   ├── xdrlib.cpython-311.opt-2.pyc
    │   │       │   ├── xdrlib.cpython-311.pyc
    │   │       │   ├── zipapp.cpython-311.opt-1.pyc
    │   │       │   ├── zipapp.cpython-311.opt-2.pyc
    │   │       │   ├── zipapp.cpython-311.pyc
    │   │       │   ├── zipfile.cpython-311.opt-1.pyc
    │   │       │   ├── zipfile.cpython-311.opt-2.pyc
    │   │       │   ├── zipfile.cpython-311.pyc
    │   │       │   ├── zipimport.cpython-311.opt-1.pyc
    │   │       │   ├── zipimport.cpython-311.opt-2.pyc
    │   │       │   └── zipimport.cpython-311.pyc
    │   │       ├── pyclbr.py
    │   │       ├── py_compile.py
    │   │       ├── _pydecimal.py
    │   │       ├── pydoc_data
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── topics.cpython-311.opt-1.pyc
    │   │       │   │   ├── topics.cpython-311.opt-2.pyc
    │   │       │   │   └── topics.cpython-311.pyc
    │   │       │   ├── _pydoc.css
    │   │       │   └── topics.py
    │   │       ├── pydoc.py
    │   │       ├── _pyio.py
    │   │       ├── queue.py
    │   │       ├── quopri.py
    │   │       ├── random.py
    │   │       ├── re
    │   │       │   ├── _casefix.py
    │   │       │   ├── _compiler.py
    │   │       │   ├── _constants.py
    │   │       │   ├── __init__.py
    │   │       │   ├── _parser.py
    │   │       │   └── __pycache__
    │   │       │       ├── _casefix.cpython-311.opt-1.pyc
    │   │       │       ├── _casefix.cpython-311.opt-2.pyc
    │   │       │       ├── _casefix.cpython-311.pyc
    │   │       │       ├── _compiler.cpython-311.opt-1.pyc
    │   │       │       ├── _compiler.cpython-311.opt-2.pyc
    │   │       │       ├── _compiler.cpython-311.pyc
    │   │       │       ├── _constants.cpython-311.opt-1.pyc
    │   │       │       ├── _constants.cpython-311.opt-2.pyc
    │   │       │       ├── _constants.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       ├── __init__.cpython-311.pyc
    │   │       │       ├── _parser.cpython-311.opt-1.pyc
    │   │       │       ├── _parser.cpython-311.opt-2.pyc
    │   │       │       └── _parser.cpython-311.pyc
    │   │       ├── reprlib.py
    │   │       ├── rlcompleter.py
    │   │       ├── runpy.py
    │   │       ├── sched.py
    │   │       ├── secrets.py
    │   │       ├── selectors.py
    │   │       ├── shelve.py
    │   │       ├── shlex.py
    │   │       ├── shutil.py
    │   │       ├── signal.py
    │   │       ├── _sitebuiltins.py
    │   │       ├── site-packages
    │   │       │   ├── _distutils_hack
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── override.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       └── override.cpython-311.pyc
    │   │       │   ├── distutils-precedence.pth
    │   │       │   ├── pip
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── _internal
    │   │       │   │   │   ├── build_env.py
    │   │       │   │   │   ├── cache.py
    │   │       │   │   │   ├── cli
    │   │       │   │   │   │   ├── autocompletion.py
    │   │       │   │   │   │   ├── base_command.py
    │   │       │   │   │   │   ├── cmdoptions.py
    │   │       │   │   │   │   ├── command_context.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── main_parser.py
    │   │       │   │   │   │   ├── main.py
    │   │       │   │   │   │   ├── parser.py
    │   │       │   │   │   │   ├── progress_bars.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── autocompletion.cpython-311.pyc
    │   │       │   │   │   │   │   ├── base_command.cpython-311.pyc
    │   │       │   │   │   │   │   ├── cmdoptions.cpython-311.pyc
    │   │       │   │   │   │   │   ├── command_context.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── main.cpython-311.pyc
    │   │       │   │   │   │   │   ├── main_parser.cpython-311.pyc
    │   │       │   │   │   │   │   ├── parser.cpython-311.pyc
    │   │       │   │   │   │   │   ├── progress_bars.cpython-311.pyc
    │   │       │   │   │   │   │   ├── req_command.cpython-311.pyc
    │   │       │   │   │   │   │   ├── spinners.cpython-311.pyc
    │   │       │   │   │   │   │   └── status_codes.cpython-311.pyc
    │   │       │   │   │   │   ├── req_command.py
    │   │       │   │   │   │   ├── spinners.py
    │   │       │   │   │   │   └── status_codes.py
    │   │       │   │   │   ├── commands
    │   │       │   │   │   │   ├── cache.py
    │   │       │   │   │   │   ├── check.py
    │   │       │   │   │   │   ├── completion.py
    │   │       │   │   │   │   ├── configuration.py
    │   │       │   │   │   │   ├── debug.py
    │   │       │   │   │   │   ├── download.py
    │   │       │   │   │   │   ├── freeze.py
    │   │       │   │   │   │   ├── hash.py
    │   │       │   │   │   │   ├── help.py
    │   │       │   │   │   │   ├── index.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── inspect.py
    │   │       │   │   │   │   ├── install.py
    │   │       │   │   │   │   ├── list.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── cache.cpython-311.pyc
    │   │       │   │   │   │   │   ├── check.cpython-311.pyc
    │   │       │   │   │   │   │   ├── completion.cpython-311.pyc
    │   │       │   │   │   │   │   ├── configuration.cpython-311.pyc
    │   │       │   │   │   │   │   ├── debug.cpython-311.pyc
    │   │       │   │   │   │   │   ├── download.cpython-311.pyc
    │   │       │   │   │   │   │   ├── freeze.cpython-311.pyc
    │   │       │   │   │   │   │   ├── hash.cpython-311.pyc
    │   │       │   │   │   │   │   ├── help.cpython-311.pyc
    │   │       │   │   │   │   │   ├── index.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── inspect.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install.cpython-311.pyc
    │   │       │   │   │   │   │   ├── list.cpython-311.pyc
    │   │       │   │   │   │   │   ├── search.cpython-311.pyc
    │   │       │   │   │   │   │   ├── show.cpython-311.pyc
    │   │       │   │   │   │   │   ├── uninstall.cpython-311.pyc
    │   │       │   │   │   │   │   └── wheel.cpython-311.pyc
    │   │       │   │   │   │   ├── search.py
    │   │       │   │   │   │   ├── show.py
    │   │       │   │   │   │   ├── uninstall.py
    │   │       │   │   │   │   └── wheel.py
    │   │       │   │   │   ├── configuration.py
    │   │       │   │   │   ├── distributions
    │   │       │   │   │   │   ├── base.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── installed.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── base.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── installed.cpython-311.pyc
    │   │       │   │   │   │   │   ├── sdist.cpython-311.pyc
    │   │       │   │   │   │   │   └── wheel.cpython-311.pyc
    │   │       │   │   │   │   ├── sdist.py
    │   │       │   │   │   │   └── wheel.py
    │   │       │   │   │   ├── exceptions.py
    │   │       │   │   │   ├── index
    │   │       │   │   │   │   ├── collector.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── package_finder.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── collector.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── package_finder.cpython-311.pyc
    │   │       │   │   │   │   │   └── sources.cpython-311.pyc
    │   │       │   │   │   │   └── sources.py
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── locations
    │   │       │   │   │   │   ├── base.py
    │   │       │   │   │   │   ├── _distutils.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── base.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _distutils.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   └── _sysconfig.cpython-311.pyc
    │   │       │   │   │   │   └── _sysconfig.py
    │   │       │   │   │   ├── main.py
    │   │       │   │   │   ├── metadata
    │   │       │   │   │   │   ├── base.py
    │   │       │   │   │   │   ├── importlib
    │   │       │   │   │   │   │   ├── _compat.py
    │   │       │   │   │   │   │   ├── _dists.py
    │   │       │   │   │   │   │   ├── _envs.py
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │       ├── _compat.cpython-311.pyc
    │   │       │   │   │   │   │       ├── _dists.cpython-311.pyc
    │   │       │   │   │   │   │       ├── _envs.cpython-311.pyc
    │   │       │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── _json.py
    │   │       │   │   │   │   ├── pkg_resources.py
    │   │       │   │   │   │   └── __pycache__
    │   │       │   │   │   │       ├── base.cpython-311.pyc
    │   │       │   │   │   │       ├── __init__.cpython-311.pyc
    │   │       │   │   │   │       ├── _json.cpython-311.pyc
    │   │       │   │   │   │       └── pkg_resources.cpython-311.pyc
    │   │       │   │   │   ├── models
    │   │       │   │   │   │   ├── candidate.py
    │   │       │   │   │   │   ├── direct_url.py
    │   │       │   │   │   │   ├── format_control.py
    │   │       │   │   │   │   ├── index.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── installation_report.py
    │   │       │   │   │   │   ├── link.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── candidate.cpython-311.pyc
    │   │       │   │   │   │   │   ├── direct_url.cpython-311.pyc
    │   │       │   │   │   │   │   ├── format_control.cpython-311.pyc
    │   │       │   │   │   │   │   ├── index.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── installation_report.cpython-311.pyc
    │   │       │   │   │   │   │   ├── link.cpython-311.pyc
    │   │       │   │   │   │   │   ├── scheme.cpython-311.pyc
    │   │       │   │   │   │   │   ├── search_scope.cpython-311.pyc
    │   │       │   │   │   │   │   ├── selection_prefs.cpython-311.pyc
    │   │       │   │   │   │   │   ├── target_python.cpython-311.pyc
    │   │       │   │   │   │   │   └── wheel.cpython-311.pyc
    │   │       │   │   │   │   ├── scheme.py
    │   │       │   │   │   │   ├── search_scope.py
    │   │       │   │   │   │   ├── selection_prefs.py
    │   │       │   │   │   │   ├── target_python.py
    │   │       │   │   │   │   └── wheel.py
    │   │       │   │   │   ├── network
    │   │       │   │   │   │   ├── auth.py
    │   │       │   │   │   │   ├── cache.py
    │   │       │   │   │   │   ├── download.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── lazy_wheel.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── auth.cpython-311.pyc
    │   │       │   │   │   │   │   ├── cache.cpython-311.pyc
    │   │       │   │   │   │   │   ├── download.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── lazy_wheel.cpython-311.pyc
    │   │       │   │   │   │   │   ├── session.cpython-311.pyc
    │   │       │   │   │   │   │   ├── utils.cpython-311.pyc
    │   │       │   │   │   │   │   └── xmlrpc.cpython-311.pyc
    │   │       │   │   │   │   ├── session.py
    │   │       │   │   │   │   ├── utils.py
    │   │       │   │   │   │   └── xmlrpc.py
    │   │       │   │   │   ├── operations
    │   │       │   │   │   │   ├── build
    │   │       │   │   │   │   │   ├── build_tracker.py
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   ├── metadata_editable.py
    │   │       │   │   │   │   │   ├── metadata_legacy.py
    │   │       │   │   │   │   │   ├── metadata.py
    │   │       │   │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   │   ├── build_tracker.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── metadata.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── metadata_editable.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── metadata_legacy.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── wheel.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── wheel_editable.cpython-311.pyc
    │   │       │   │   │   │   │   │   └── wheel_legacy.cpython-311.pyc
    │   │       │   │   │   │   │   ├── wheel_editable.py
    │   │       │   │   │   │   │   ├── wheel_legacy.py
    │   │       │   │   │   │   │   └── wheel.py
    │   │       │   │   │   │   ├── check.py
    │   │       │   │   │   │   ├── freeze.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── install
    │   │       │   │   │   │   │   ├── editable_legacy.py
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   │   ├── editable_legacy.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   │   └── wheel.cpython-311.pyc
    │   │       │   │   │   │   │   └── wheel.py
    │   │       │   │   │   │   ├── prepare.py
    │   │       │   │   │   │   └── __pycache__
    │   │       │   │   │   │       ├── check.cpython-311.pyc
    │   │       │   │   │   │       ├── freeze.cpython-311.pyc
    │   │       │   │   │   │       ├── __init__.cpython-311.pyc
    │   │       │   │   │   │       └── prepare.cpython-311.pyc
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── build_env.cpython-311.pyc
    │   │       │   │   │   │   ├── cache.cpython-311.pyc
    │   │       │   │   │   │   ├── configuration.cpython-311.pyc
    │   │       │   │   │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── main.cpython-311.pyc
    │   │       │   │   │   │   ├── pyproject.cpython-311.pyc
    │   │       │   │   │   │   ├── self_outdated_check.cpython-311.pyc
    │   │       │   │   │   │   └── wheel_builder.cpython-311.pyc
    │   │       │   │   │   ├── pyproject.py
    │   │       │   │   │   ├── req
    │   │       │   │   │   │   ├── constructors.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── constructors.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── req_file.cpython-311.pyc
    │   │       │   │   │   │   │   ├── req_install.cpython-311.pyc
    │   │       │   │   │   │   │   ├── req_set.cpython-311.pyc
    │   │       │   │   │   │   │   └── req_uninstall.cpython-311.pyc
    │   │       │   │   │   │   ├── req_file.py
    │   │       │   │   │   │   ├── req_install.py
    │   │       │   │   │   │   ├── req_set.py
    │   │       │   │   │   │   └── req_uninstall.py
    │   │       │   │   │   ├── resolution
    │   │       │   │   │   │   ├── base.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── legacy
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   │   └── resolver.cpython-311.pyc
    │   │       │   │   │   │   │   └── resolver.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── base.cpython-311.pyc
    │   │       │   │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   │   └── resolvelib
    │   │       │   │   │   │       ├── base.py
    │   │       │   │   │   │       ├── candidates.py
    │   │       │   │   │   │       ├── factory.py
    │   │       │   │   │   │       ├── found_candidates.py
    │   │       │   │   │   │       ├── __init__.py
    │   │       │   │   │   │       ├── provider.py
    │   │       │   │   │   │       ├── __pycache__
    │   │       │   │   │   │       │   ├── base.cpython-311.pyc
    │   │       │   │   │   │       │   ├── candidates.cpython-311.pyc
    │   │       │   │   │   │       │   ├── factory.cpython-311.pyc
    │   │       │   │   │   │       │   ├── found_candidates.cpython-311.pyc
    │   │       │   │   │   │       │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │       │   ├── provider.cpython-311.pyc
    │   │       │   │   │   │       │   ├── reporter.cpython-311.pyc
    │   │       │   │   │   │       │   ├── requirements.cpython-311.pyc
    │   │       │   │   │   │       │   └── resolver.cpython-311.pyc
    │   │       │   │   │   │       ├── reporter.py
    │   │       │   │   │   │       ├── requirements.py
    │   │       │   │   │   │       └── resolver.py
    │   │       │   │   │   ├── self_outdated_check.py
    │   │       │   │   │   ├── utils
    │   │       │   │   │   │   ├── appdirs.py
    │   │       │   │   │   │   ├── compatibility_tags.py
    │   │       │   │   │   │   ├── compat.py
    │   │       │   │   │   │   ├── datetime.py
    │   │       │   │   │   │   ├── deprecation.py
    │   │       │   │   │   │   ├── direct_url_helpers.py
    │   │       │   │   │   │   ├── egg_link.py
    │   │       │   │   │   │   ├── encoding.py
    │   │       │   │   │   │   ├── entrypoints.py
    │   │       │   │   │   │   ├── filesystem.py
    │   │       │   │   │   │   ├── filetypes.py
    │   │       │   │   │   │   ├── glibc.py
    │   │       │   │   │   │   ├── hashes.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── inject_securetransport.py
    │   │       │   │   │   │   ├── _jaraco_text.py
    │   │       │   │   │   │   ├── logging.py
    │   │       │   │   │   │   ├── _log.py
    │   │       │   │   │   │   ├── misc.py
    │   │       │   │   │   │   ├── models.py
    │   │       │   │   │   │   ├── packaging.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── appdirs.cpython-311.pyc
    │   │       │   │   │   │   │   ├── compat.cpython-311.pyc
    │   │       │   │   │   │   │   ├── compatibility_tags.cpython-311.pyc
    │   │       │   │   │   │   │   ├── datetime.cpython-311.pyc
    │   │       │   │   │   │   │   ├── deprecation.cpython-311.pyc
    │   │       │   │   │   │   │   ├── direct_url_helpers.cpython-311.pyc
    │   │       │   │   │   │   │   ├── egg_link.cpython-311.pyc
    │   │       │   │   │   │   │   ├── encoding.cpython-311.pyc
    │   │       │   │   │   │   │   ├── entrypoints.cpython-311.pyc
    │   │       │   │   │   │   │   ├── filesystem.cpython-311.pyc
    │   │       │   │   │   │   │   ├── filetypes.cpython-311.pyc
    │   │       │   │   │   │   │   ├── glibc.cpython-311.pyc
    │   │       │   │   │   │   │   ├── hashes.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── inject_securetransport.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _jaraco_text.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _log.cpython-311.pyc
    │   │       │   │   │   │   │   ├── logging.cpython-311.pyc
    │   │       │   │   │   │   │   ├── misc.cpython-311.pyc
    │   │       │   │   │   │   │   ├── models.cpython-311.pyc
    │   │       │   │   │   │   │   ├── packaging.cpython-311.pyc
    │   │       │   │   │   │   │   ├── setuptools_build.cpython-311.pyc
    │   │       │   │   │   │   │   ├── subprocess.cpython-311.pyc
    │   │       │   │   │   │   │   ├── temp_dir.cpython-311.pyc
    │   │       │   │   │   │   │   ├── unpacking.cpython-311.pyc
    │   │       │   │   │   │   │   ├── urls.cpython-311.pyc
    │   │       │   │   │   │   │   ├── virtualenv.cpython-311.pyc
    │   │       │   │   │   │   │   └── wheel.cpython-311.pyc
    │   │       │   │   │   │   ├── setuptools_build.py
    │   │       │   │   │   │   ├── subprocess.py
    │   │       │   │   │   │   ├── temp_dir.py
    │   │       │   │   │   │   ├── unpacking.py
    │   │       │   │   │   │   ├── urls.py
    │   │       │   │   │   │   ├── virtualenv.py
    │   │       │   │   │   │   └── wheel.py
    │   │       │   │   │   ├── vcs
    │   │       │   │   │   │   ├── bazaar.py
    │   │       │   │   │   │   ├── git.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── mercurial.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── bazaar.cpython-311.pyc
    │   │       │   │   │   │   │   ├── git.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── mercurial.cpython-311.pyc
    │   │       │   │   │   │   │   ├── subversion.cpython-311.pyc
    │   │       │   │   │   │   │   └── versioncontrol.cpython-311.pyc
    │   │       │   │   │   │   ├── subversion.py
    │   │       │   │   │   │   └── versioncontrol.py
    │   │       │   │   │   └── wheel_builder.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pip-runner__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   └── __pip-runner__.cpython-311.pyc
    │   │       │   │   ├── py.typed
    │   │       │   │   └── _vendor
    │   │       │   │       ├── cachecontrol
    │   │       │   │       │   ├── adapter.py
    │   │       │   │       │   ├── cache.py
    │   │       │   │       │   ├── caches
    │   │       │   │       │   │   ├── file_cache.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── file_cache.cpython-311.pyc
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   └── redis_cache.cpython-311.pyc
    │   │       │   │       │   │   └── redis_cache.py
    │   │       │   │       │   ├── _cmd.py
    │   │       │   │       │   ├── compat.py
    │   │       │   │       │   ├── controller.py
    │   │       │   │       │   ├── filewrapper.py
    │   │       │   │       │   ├── heuristics.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── adapter.cpython-311.pyc
    │   │       │   │       │   │   ├── cache.cpython-311.pyc
    │   │       │   │       │   │   ├── _cmd.cpython-311.pyc
    │   │       │   │       │   │   ├── compat.cpython-311.pyc
    │   │       │   │       │   │   ├── controller.cpython-311.pyc
    │   │       │   │       │   │   ├── filewrapper.cpython-311.pyc
    │   │       │   │       │   │   ├── heuristics.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── serialize.cpython-311.pyc
    │   │       │   │       │   │   └── wrapper.cpython-311.pyc
    │   │       │   │       │   ├── serialize.py
    │   │       │   │       │   └── wrapper.py
    │   │       │   │       ├── certifi
    │   │       │   │       │   ├── cacert.pem
    │   │       │   │       │   ├── core.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __main__.py
    │   │       │   │       │   └── __pycache__
    │   │       │   │       │       ├── core.cpython-311.pyc
    │   │       │   │       │       ├── __init__.cpython-311.pyc
    │   │       │   │       │       └── __main__.cpython-311.pyc
    │   │       │   │       ├── chardet
    │   │       │   │       │   ├── big5freq.py
    │   │       │   │       │   ├── big5prober.py
    │   │       │   │       │   ├── chardistribution.py
    │   │       │   │       │   ├── charsetgroupprober.py
    │   │       │   │       │   ├── charsetprober.py
    │   │       │   │       │   ├── cli
    │   │       │   │       │   │   ├── chardetect.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       ├── chardetect.cpython-311.pyc
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── codingstatemachinedict.py
    │   │       │   │       │   ├── codingstatemachine.py
    │   │       │   │       │   ├── cp949prober.py
    │   │       │   │       │   ├── enums.py
    │   │       │   │       │   ├── escprober.py
    │   │       │   │       │   ├── escsm.py
    │   │       │   │       │   ├── eucjpprober.py
    │   │       │   │       │   ├── euckrfreq.py
    │   │       │   │       │   ├── euckrprober.py
    │   │       │   │       │   ├── euctwfreq.py
    │   │       │   │       │   ├── euctwprober.py
    │   │       │   │       │   ├── gb2312freq.py
    │   │       │   │       │   ├── gb2312prober.py
    │   │       │   │       │   ├── hebrewprober.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── jisfreq.py
    │   │       │   │       │   ├── johabfreq.py
    │   │       │   │       │   ├── johabprober.py
    │   │       │   │       │   ├── jpcntx.py
    │   │       │   │       │   ├── langbulgarianmodel.py
    │   │       │   │       │   ├── langgreekmodel.py
    │   │       │   │       │   ├── langhebrewmodel.py
    │   │       │   │       │   ├── langhungarianmodel.py
    │   │       │   │       │   ├── langrussianmodel.py
    │   │       │   │       │   ├── langthaimodel.py
    │   │       │   │       │   ├── langturkishmodel.py
    │   │       │   │       │   ├── latin1prober.py
    │   │       │   │       │   ├── macromanprober.py
    │   │       │   │       │   ├── mbcharsetprober.py
    │   │       │   │       │   ├── mbcsgroupprober.py
    │   │       │   │       │   ├── mbcssm.py
    │   │       │   │       │   ├── metadata
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── languages.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       │   │       └── languages.cpython-311.pyc
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── big5freq.cpython-311.pyc
    │   │       │   │       │   │   ├── big5prober.cpython-311.pyc
    │   │       │   │       │   │   ├── chardistribution.cpython-311.pyc
    │   │       │   │       │   │   ├── charsetgroupprober.cpython-311.pyc
    │   │       │   │       │   │   ├── charsetprober.cpython-311.pyc
    │   │       │   │       │   │   ├── codingstatemachine.cpython-311.pyc
    │   │       │   │       │   │   ├── codingstatemachinedict.cpython-311.pyc
    │   │       │   │       │   │   ├── cp949prober.cpython-311.pyc
    │   │       │   │       │   │   ├── enums.cpython-311.pyc
    │   │       │   │       │   │   ├── escprober.cpython-311.pyc
    │   │       │   │       │   │   ├── escsm.cpython-311.pyc
    │   │       │   │       │   │   ├── eucjpprober.cpython-311.pyc
    │   │       │   │       │   │   ├── euckrfreq.cpython-311.pyc
    │   │       │   │       │   │   ├── euckrprober.cpython-311.pyc
    │   │       │   │       │   │   ├── euctwfreq.cpython-311.pyc
    │   │       │   │       │   │   ├── euctwprober.cpython-311.pyc
    │   │       │   │       │   │   ├── gb2312freq.cpython-311.pyc
    │   │       │   │       │   │   ├── gb2312prober.cpython-311.pyc
    │   │       │   │       │   │   ├── hebrewprober.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── jisfreq.cpython-311.pyc
    │   │       │   │       │   │   ├── johabfreq.cpython-311.pyc
    │   │       │   │       │   │   ├── johabprober.cpython-311.pyc
    │   │       │   │       │   │   ├── jpcntx.cpython-311.pyc
    │   │       │   │       │   │   ├── langbulgarianmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langgreekmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langhebrewmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langhungarianmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langrussianmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langthaimodel.cpython-311.pyc
    │   │       │   │       │   │   ├── langturkishmodel.cpython-311.pyc
    │   │       │   │       │   │   ├── latin1prober.cpython-311.pyc
    │   │       │   │       │   │   ├── macromanprober.cpython-311.pyc
    │   │       │   │       │   │   ├── mbcharsetprober.cpython-311.pyc
    │   │       │   │       │   │   ├── mbcsgroupprober.cpython-311.pyc
    │   │       │   │       │   │   ├── mbcssm.cpython-311.pyc
    │   │       │   │       │   │   ├── resultdict.cpython-311.pyc
    │   │       │   │       │   │   ├── sbcharsetprober.cpython-311.pyc
    │   │       │   │       │   │   ├── sbcsgroupprober.cpython-311.pyc
    │   │       │   │       │   │   ├── sjisprober.cpython-311.pyc
    │   │       │   │       │   │   ├── universaldetector.cpython-311.pyc
    │   │       │   │       │   │   ├── utf1632prober.cpython-311.pyc
    │   │       │   │       │   │   ├── utf8prober.cpython-311.pyc
    │   │       │   │       │   │   └── version.cpython-311.pyc
    │   │       │   │       │   ├── resultdict.py
    │   │       │   │       │   ├── sbcharsetprober.py
    │   │       │   │       │   ├── sbcsgroupprober.py
    │   │       │   │       │   ├── sjisprober.py
    │   │       │   │       │   ├── universaldetector.py
    │   │       │   │       │   ├── utf1632prober.py
    │   │       │   │       │   ├── utf8prober.py
    │   │       │   │       │   └── version.py
    │   │       │   │       ├── colorama
    │   │       │   │       │   ├── ansi.py
    │   │       │   │       │   ├── ansitowin32.py
    │   │       │   │       │   ├── initialise.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── ansi.cpython-311.pyc
    │   │       │   │       │   │   ├── ansitowin32.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── initialise.cpython-311.pyc
    │   │       │   │       │   │   ├── win32.cpython-311.pyc
    │   │       │   │       │   │   └── winterm.cpython-311.pyc
    │   │       │   │       │   ├── tests
    │   │       │   │       │   │   ├── ansi_test.py
    │   │       │   │       │   │   ├── ansitowin32_test.py
    │   │       │   │       │   │   ├── initialise_test.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── isatty_test.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── ansi_test.cpython-311.pyc
    │   │       │   │       │   │   │   ├── ansitowin32_test.cpython-311.pyc
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   ├── initialise_test.cpython-311.pyc
    │   │       │   │       │   │   │   ├── isatty_test.cpython-311.pyc
    │   │       │   │       │   │   │   ├── utils.cpython-311.pyc
    │   │       │   │       │   │   │   └── winterm_test.cpython-311.pyc
    │   │       │   │       │   │   ├── utils.py
    │   │       │   │       │   │   └── winterm_test.py
    │   │       │   │       │   ├── win32.py
    │   │       │   │       │   └── winterm.py
    │   │       │   │       ├── distlib
    │   │       │   │       │   ├── compat.py
    │   │       │   │       │   ├── database.py
    │   │       │   │       │   ├── index.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── locators.py
    │   │       │   │       │   ├── manifest.py
    │   │       │   │       │   ├── markers.py
    │   │       │   │       │   ├── metadata.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── compat.cpython-311.pyc
    │   │       │   │       │   │   ├── database.cpython-311.pyc
    │   │       │   │       │   │   ├── index.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── locators.cpython-311.pyc
    │   │       │   │       │   │   ├── manifest.cpython-311.pyc
    │   │       │   │       │   │   ├── markers.cpython-311.pyc
    │   │       │   │       │   │   ├── metadata.cpython-311.pyc
    │   │       │   │       │   │   ├── resources.cpython-311.pyc
    │   │       │   │       │   │   ├── scripts.cpython-311.pyc
    │   │       │   │       │   │   ├── util.cpython-311.pyc
    │   │       │   │       │   │   ├── version.cpython-311.pyc
    │   │       │   │       │   │   └── wheel.cpython-311.pyc
    │   │       │   │       │   ├── resources.py
    │   │       │   │       │   ├── scripts.py
    │   │       │   │       │   ├── t32.exe
    │   │       │   │       │   ├── t64-arm.exe
    │   │       │   │       │   ├── t64.exe
    │   │       │   │       │   ├── util.py
    │   │       │   │       │   ├── version.py
    │   │       │   │       │   ├── w32.exe
    │   │       │   │       │   ├── w64-arm.exe
    │   │       │   │       │   ├── w64.exe
    │   │       │   │       │   └── wheel.py
    │   │       │   │       ├── distro
    │   │       │   │       │   ├── distro.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __main__.py
    │   │       │   │       │   └── __pycache__
    │   │       │   │       │       ├── distro.cpython-311.pyc
    │   │       │   │       │       ├── __init__.cpython-311.pyc
    │   │       │   │       │       └── __main__.cpython-311.pyc
    │   │       │   │       ├── idna
    │   │       │   │       │   ├── codec.py
    │   │       │   │       │   ├── compat.py
    │   │       │   │       │   ├── core.py
    │   │       │   │       │   ├── idnadata.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── intranges.py
    │   │       │   │       │   ├── package_data.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── codec.cpython-311.pyc
    │   │       │   │       │   │   ├── compat.cpython-311.pyc
    │   │       │   │       │   │   ├── core.cpython-311.pyc
    │   │       │   │       │   │   ├── idnadata.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── intranges.cpython-311.pyc
    │   │       │   │       │   │   ├── package_data.cpython-311.pyc
    │   │       │   │       │   │   └── uts46data.cpython-311.pyc
    │   │       │   │       │   └── uts46data.py
    │   │       │   │       ├── __init__.py
    │   │       │   │       ├── msgpack
    │   │       │   │       │   ├── exceptions.py
    │   │       │   │       │   ├── ext.py
    │   │       │   │       │   ├── fallback.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   └── __pycache__
    │   │       │   │       │       ├── exceptions.cpython-311.pyc
    │   │       │   │       │       ├── ext.cpython-311.pyc
    │   │       │   │       │       ├── fallback.cpython-311.pyc
    │   │       │   │       │       └── __init__.cpython-311.pyc
    │   │       │   │       ├── packaging
    │   │       │   │       │   ├── __about__.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _manylinux.py
    │   │       │   │       │   ├── markers.py
    │   │       │   │       │   ├── _musllinux.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── __about__.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _manylinux.cpython-311.pyc
    │   │       │   │       │   │   ├── markers.cpython-311.pyc
    │   │       │   │       │   │   ├── _musllinux.cpython-311.pyc
    │   │       │   │       │   │   ├── requirements.cpython-311.pyc
    │   │       │   │       │   │   ├── specifiers.cpython-311.pyc
    │   │       │   │       │   │   ├── _structures.cpython-311.pyc
    │   │       │   │       │   │   ├── tags.cpython-311.pyc
    │   │       │   │       │   │   ├── utils.cpython-311.pyc
    │   │       │   │       │   │   └── version.cpython-311.pyc
    │   │       │   │       │   ├── requirements.py
    │   │       │   │       │   ├── specifiers.py
    │   │       │   │       │   ├── _structures.py
    │   │       │   │       │   ├── tags.py
    │   │       │   │       │   ├── utils.py
    │   │       │   │       │   └── version.py
    │   │       │   │       ├── pkg_resources
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   └── __pycache__
    │   │       │   │       │       └── __init__.cpython-311.pyc
    │   │       │   │       ├── platformdirs
    │   │       │   │       │   ├── android.py
    │   │       │   │       │   ├── api.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── macos.py
    │   │       │   │       │   ├── __main__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── android.cpython-311.pyc
    │   │       │   │       │   │   ├── api.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── macos.cpython-311.pyc
    │   │       │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │       │   │   ├── unix.cpython-311.pyc
    │   │       │   │       │   │   ├── version.cpython-311.pyc
    │   │       │   │       │   │   └── windows.cpython-311.pyc
    │   │       │   │       │   ├── unix.py
    │   │       │   │       │   ├── version.py
    │   │       │   │       │   └── windows.py
    │   │       │   │       ├── __pycache__
    │   │       │   │       │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   ├── six.cpython-311.pyc
    │   │       │   │       │   └── typing_extensions.cpython-311.pyc
    │   │       │   │       ├── pygments
    │   │       │   │       │   ├── cmdline.py
    │   │       │   │       │   ├── console.py
    │   │       │   │       │   ├── filter.py
    │   │       │   │       │   ├── filters
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── formatter.py
    │   │       │   │       │   ├── formatters
    │   │       │   │       │   │   ├── bbcode.py
    │   │       │   │       │   │   ├── groff.py
    │   │       │   │       │   │   ├── html.py
    │   │       │   │       │   │   ├── img.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── irc.py
    │   │       │   │       │   │   ├── latex.py
    │   │       │   │       │   │   ├── _mapping.py
    │   │       │   │       │   │   ├── other.py
    │   │       │   │       │   │   ├── pangomarkup.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── bbcode.cpython-311.pyc
    │   │       │   │       │   │   │   ├── groff.cpython-311.pyc
    │   │       │   │       │   │   │   ├── html.cpython-311.pyc
    │   │       │   │       │   │   │   ├── img.cpython-311.pyc
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   ├── irc.cpython-311.pyc
    │   │       │   │       │   │   │   ├── latex.cpython-311.pyc
    │   │       │   │       │   │   │   ├── _mapping.cpython-311.pyc
    │   │       │   │       │   │   │   ├── other.cpython-311.pyc
    │   │       │   │       │   │   │   ├── pangomarkup.cpython-311.pyc
    │   │       │   │       │   │   │   ├── rtf.cpython-311.pyc
    │   │       │   │       │   │   │   ├── svg.cpython-311.pyc
    │   │       │   │       │   │   │   ├── terminal256.cpython-311.pyc
    │   │       │   │       │   │   │   └── terminal.cpython-311.pyc
    │   │       │   │       │   │   ├── rtf.py
    │   │       │   │       │   │   ├── svg.py
    │   │       │   │       │   │   ├── terminal256.py
    │   │       │   │       │   │   └── terminal.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── lexer.py
    │   │       │   │       │   ├── lexers
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── _mapping.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   ├── _mapping.cpython-311.pyc
    │   │       │   │       │   │   │   └── python.cpython-311.pyc
    │   │       │   │       │   │   └── python.py
    │   │       │   │       │   ├── __main__.py
    │   │       │   │       │   ├── modeline.py
    │   │       │   │       │   ├── plugin.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── cmdline.cpython-311.pyc
    │   │       │   │       │   │   ├── console.cpython-311.pyc
    │   │       │   │       │   │   ├── filter.cpython-311.pyc
    │   │       │   │       │   │   ├── formatter.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── lexer.cpython-311.pyc
    │   │       │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │       │   │   ├── modeline.cpython-311.pyc
    │   │       │   │       │   │   ├── plugin.cpython-311.pyc
    │   │       │   │       │   │   ├── regexopt.cpython-311.pyc
    │   │       │   │       │   │   ├── scanner.cpython-311.pyc
    │   │       │   │       │   │   ├── sphinxext.cpython-311.pyc
    │   │       │   │       │   │   ├── style.cpython-311.pyc
    │   │       │   │       │   │   ├── token.cpython-311.pyc
    │   │       │   │       │   │   ├── unistring.cpython-311.pyc
    │   │       │   │       │   │   └── util.cpython-311.pyc
    │   │       │   │       │   ├── regexopt.py
    │   │       │   │       │   ├── scanner.py
    │   │       │   │       │   ├── sphinxext.py
    │   │       │   │       │   ├── style.py
    │   │       │   │       │   ├── styles
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── token.py
    │   │       │   │       │   ├── unistring.py
    │   │       │   │       │   └── util.py
    │   │       │   │       ├── pyparsing
    │   │       │   │       │   ├── actions.py
    │   │       │   │       │   ├── common.py
    │   │       │   │       │   ├── core.py
    │   │       │   │       │   ├── diagram
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── exceptions.py
    │   │       │   │       │   ├── helpers.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── actions.cpython-311.pyc
    │   │       │   │       │   │   ├── common.cpython-311.pyc
    │   │       │   │       │   │   ├── core.cpython-311.pyc
    │   │       │   │       │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │       │   │   ├── helpers.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── results.cpython-311.pyc
    │   │       │   │       │   │   ├── testing.cpython-311.pyc
    │   │       │   │       │   │   ├── unicode.cpython-311.pyc
    │   │       │   │       │   │   └── util.cpython-311.pyc
    │   │       │   │       │   ├── results.py
    │   │       │   │       │   ├── testing.py
    │   │       │   │       │   ├── unicode.py
    │   │       │   │       │   └── util.py
    │   │       │   │       ├── pyproject_hooks
    │   │       │   │       │   ├── _compat.py
    │   │       │   │       │   ├── _impl.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _in_process
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── _in_process.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       │   │       └── _in_process.cpython-311.pyc
    │   │       │   │       │   └── __pycache__
    │   │       │   │       │       ├── _compat.cpython-311.pyc
    │   │       │   │       │       ├── _impl.cpython-311.pyc
    │   │       │   │       │       └── __init__.cpython-311.pyc
    │   │       │   │       ├── requests
    │   │       │   │       │   ├── adapters.py
    │   │       │   │       │   ├── api.py
    │   │       │   │       │   ├── auth.py
    │   │       │   │       │   ├── certs.py
    │   │       │   │       │   ├── compat.py
    │   │       │   │       │   ├── cookies.py
    │   │       │   │       │   ├── exceptions.py
    │   │       │   │       │   ├── help.py
    │   │       │   │       │   ├── hooks.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _internal_utils.py
    │   │       │   │       │   ├── models.py
    │   │       │   │       │   ├── packages.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── adapters.cpython-311.pyc
    │   │       │   │       │   │   ├── api.cpython-311.pyc
    │   │       │   │       │   │   ├── auth.cpython-311.pyc
    │   │       │   │       │   │   ├── certs.cpython-311.pyc
    │   │       │   │       │   │   ├── compat.cpython-311.pyc
    │   │       │   │       │   │   ├── cookies.cpython-311.pyc
    │   │       │   │       │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │       │   │   ├── help.cpython-311.pyc
    │   │       │   │       │   │   ├── hooks.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _internal_utils.cpython-311.pyc
    │   │       │   │       │   │   ├── models.cpython-311.pyc
    │   │       │   │       │   │   ├── packages.cpython-311.pyc
    │   │       │   │       │   │   ├── sessions.cpython-311.pyc
    │   │       │   │       │   │   ├── status_codes.cpython-311.pyc
    │   │       │   │       │   │   ├── structures.cpython-311.pyc
    │   │       │   │       │   │   ├── utils.cpython-311.pyc
    │   │       │   │       │   │   └── __version__.cpython-311.pyc
    │   │       │   │       │   ├── sessions.py
    │   │       │   │       │   ├── status_codes.py
    │   │       │   │       │   ├── structures.py
    │   │       │   │       │   ├── utils.py
    │   │       │   │       │   └── __version__.py
    │   │       │   │       ├── resolvelib
    │   │       │   │       │   ├── compat
    │   │       │   │       │   │   ├── collections_abc.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       ├── collections_abc.cpython-311.pyc
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── providers.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── providers.cpython-311.pyc
    │   │       │   │       │   │   ├── reporters.cpython-311.pyc
    │   │       │   │       │   │   ├── resolvers.cpython-311.pyc
    │   │       │   │       │   │   └── structs.cpython-311.pyc
    │   │       │   │       │   ├── reporters.py
    │   │       │   │       │   ├── resolvers.py
    │   │       │   │       │   └── structs.py
    │   │       │   │       ├── rich
    │   │       │   │       │   ├── abc.py
    │   │       │   │       │   ├── align.py
    │   │       │   │       │   ├── ansi.py
    │   │       │   │       │   ├── bar.py
    │   │       │   │       │   ├── box.py
    │   │       │   │       │   ├── cells.py
    │   │       │   │       │   ├── _cell_widths.py
    │   │       │   │       │   ├── color.py
    │   │       │   │       │   ├── color_triplet.py
    │   │       │   │       │   ├── columns.py
    │   │       │   │       │   ├── console.py
    │   │       │   │       │   ├── constrain.py
    │   │       │   │       │   ├── containers.py
    │   │       │   │       │   ├── control.py
    │   │       │   │       │   ├── default_styles.py
    │   │       │   │       │   ├── diagnose.py
    │   │       │   │       │   ├── _emoji_codes.py
    │   │       │   │       │   ├── emoji.py
    │   │       │   │       │   ├── _emoji_replace.py
    │   │       │   │       │   ├── errors.py
    │   │       │   │       │   ├── _export_format.py
    │   │       │   │       │   ├── _extension.py
    │   │       │   │       │   ├── _fileno.py
    │   │       │   │       │   ├── file_proxy.py
    │   │       │   │       │   ├── filesize.py
    │   │       │   │       │   ├── highlighter.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _inspect.py
    │   │       │   │       │   ├── json.py
    │   │       │   │       │   ├── jupyter.py
    │   │       │   │       │   ├── layout.py
    │   │       │   │       │   ├── live.py
    │   │       │   │       │   ├── live_render.py
    │   │       │   │       │   ├── logging.py
    │   │       │   │       │   ├── _log_render.py
    │   │       │   │       │   ├── _loop.py
    │   │       │   │       │   ├── __main__.py
    │   │       │   │       │   ├── markup.py
    │   │       │   │       │   ├── measure.py
    │   │       │   │       │   ├── _null_file.py
    │   │       │   │       │   ├── padding.py
    │   │       │   │       │   ├── pager.py
    │   │       │   │       │   ├── palette.py
    │   │       │   │       │   ├── _palettes.py
    │   │       │   │       │   ├── panel.py
    │   │       │   │       │   ├── _pick.py
    │   │       │   │       │   ├── pretty.py
    │   │       │   │       │   ├── progress_bar.py
    │   │       │   │       │   ├── progress.py
    │   │       │   │       │   ├── prompt.py
    │   │       │   │       │   ├── protocol.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── abc.cpython-311.pyc
    │   │       │   │       │   │   ├── align.cpython-311.pyc
    │   │       │   │       │   │   ├── ansi.cpython-311.pyc
    │   │       │   │       │   │   ├── bar.cpython-311.pyc
    │   │       │   │       │   │   ├── box.cpython-311.pyc
    │   │       │   │       │   │   ├── cells.cpython-311.pyc
    │   │       │   │       │   │   ├── _cell_widths.cpython-311.pyc
    │   │       │   │       │   │   ├── color.cpython-311.pyc
    │   │       │   │       │   │   ├── color_triplet.cpython-311.pyc
    │   │       │   │       │   │   ├── columns.cpython-311.pyc
    │   │       │   │       │   │   ├── console.cpython-311.pyc
    │   │       │   │       │   │   ├── constrain.cpython-311.pyc
    │   │       │   │       │   │   ├── containers.cpython-311.pyc
    │   │       │   │       │   │   ├── control.cpython-311.pyc
    │   │       │   │       │   │   ├── default_styles.cpython-311.pyc
    │   │       │   │       │   │   ├── diagnose.cpython-311.pyc
    │   │       │   │       │   │   ├── _emoji_codes.cpython-311.pyc
    │   │       │   │       │   │   ├── emoji.cpython-311.pyc
    │   │       │   │       │   │   ├── _emoji_replace.cpython-311.pyc
    │   │       │   │       │   │   ├── errors.cpython-311.pyc
    │   │       │   │       │   │   ├── _export_format.cpython-311.pyc
    │   │       │   │       │   │   ├── _extension.cpython-311.pyc
    │   │       │   │       │   │   ├── _fileno.cpython-311.pyc
    │   │       │   │       │   │   ├── file_proxy.cpython-311.pyc
    │   │       │   │       │   │   ├── filesize.cpython-311.pyc
    │   │       │   │       │   │   ├── highlighter.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _inspect.cpython-311.pyc
    │   │       │   │       │   │   ├── json.cpython-311.pyc
    │   │       │   │       │   │   ├── jupyter.cpython-311.pyc
    │   │       │   │       │   │   ├── layout.cpython-311.pyc
    │   │       │   │       │   │   ├── live.cpython-311.pyc
    │   │       │   │       │   │   ├── live_render.cpython-311.pyc
    │   │       │   │       │   │   ├── logging.cpython-311.pyc
    │   │       │   │       │   │   ├── _log_render.cpython-311.pyc
    │   │       │   │       │   │   ├── _loop.cpython-311.pyc
    │   │       │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │       │   │   ├── markup.cpython-311.pyc
    │   │       │   │       │   │   ├── measure.cpython-311.pyc
    │   │       │   │       │   │   ├── _null_file.cpython-311.pyc
    │   │       │   │       │   │   ├── padding.cpython-311.pyc
    │   │       │   │       │   │   ├── pager.cpython-311.pyc
    │   │       │   │       │   │   ├── palette.cpython-311.pyc
    │   │       │   │       │   │   ├── _palettes.cpython-311.pyc
    │   │       │   │       │   │   ├── panel.cpython-311.pyc
    │   │       │   │       │   │   ├── _pick.cpython-311.pyc
    │   │       │   │       │   │   ├── pretty.cpython-311.pyc
    │   │       │   │       │   │   ├── progress_bar.cpython-311.pyc
    │   │       │   │       │   │   ├── progress.cpython-311.pyc
    │   │       │   │       │   │   ├── prompt.cpython-311.pyc
    │   │       │   │       │   │   ├── protocol.cpython-311.pyc
    │   │       │   │       │   │   ├── _ratio.cpython-311.pyc
    │   │       │   │       │   │   ├── region.cpython-311.pyc
    │   │       │   │       │   │   ├── repr.cpython-311.pyc
    │   │       │   │       │   │   ├── rule.cpython-311.pyc
    │   │       │   │       │   │   ├── scope.cpython-311.pyc
    │   │       │   │       │   │   ├── screen.cpython-311.pyc
    │   │       │   │       │   │   ├── segment.cpython-311.pyc
    │   │       │   │       │   │   ├── spinner.cpython-311.pyc
    │   │       │   │       │   │   ├── _spinners.cpython-311.pyc
    │   │       │   │       │   │   ├── _stack.cpython-311.pyc
    │   │       │   │       │   │   ├── status.cpython-311.pyc
    │   │       │   │       │   │   ├── style.cpython-311.pyc
    │   │       │   │       │   │   ├── styled.cpython-311.pyc
    │   │       │   │       │   │   ├── syntax.cpython-311.pyc
    │   │       │   │       │   │   ├── table.cpython-311.pyc
    │   │       │   │       │   │   ├── terminal_theme.cpython-311.pyc
    │   │       │   │       │   │   ├── text.cpython-311.pyc
    │   │       │   │       │   │   ├── theme.cpython-311.pyc
    │   │       │   │       │   │   ├── themes.cpython-311.pyc
    │   │       │   │       │   │   ├── _timer.cpython-311.pyc
    │   │       │   │       │   │   ├── traceback.cpython-311.pyc
    │   │       │   │       │   │   ├── tree.cpython-311.pyc
    │   │       │   │       │   │   ├── _win32_console.cpython-311.pyc
    │   │       │   │       │   │   ├── _windows.cpython-311.pyc
    │   │       │   │       │   │   ├── _windows_renderer.cpython-311.pyc
    │   │       │   │       │   │   └── _wrap.cpython-311.pyc
    │   │       │   │       │   ├── _ratio.py
    │   │       │   │       │   ├── region.py
    │   │       │   │       │   ├── repr.py
    │   │       │   │       │   ├── rule.py
    │   │       │   │       │   ├── scope.py
    │   │       │   │       │   ├── screen.py
    │   │       │   │       │   ├── segment.py
    │   │       │   │       │   ├── spinner.py
    │   │       │   │       │   ├── _spinners.py
    │   │       │   │       │   ├── _stack.py
    │   │       │   │       │   ├── status.py
    │   │       │   │       │   ├── styled.py
    │   │       │   │       │   ├── style.py
    │   │       │   │       │   ├── syntax.py
    │   │       │   │       │   ├── table.py
    │   │       │   │       │   ├── terminal_theme.py
    │   │       │   │       │   ├── text.py
    │   │       │   │       │   ├── theme.py
    │   │       │   │       │   ├── themes.py
    │   │       │   │       │   ├── _timer.py
    │   │       │   │       │   ├── traceback.py
    │   │       │   │       │   ├── tree.py
    │   │       │   │       │   ├── _win32_console.py
    │   │       │   │       │   ├── _windows.py
    │   │       │   │       │   ├── _windows_renderer.py
    │   │       │   │       │   └── _wrap.py
    │   │       │   │       ├── six.py
    │   │       │   │       ├── tenacity
    │   │       │   │       │   ├── after.py
    │   │       │   │       │   ├── _asyncio.py
    │   │       │   │       │   ├── before.py
    │   │       │   │       │   ├── before_sleep.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── nap.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── after.cpython-311.pyc
    │   │       │   │       │   │   ├── _asyncio.cpython-311.pyc
    │   │       │   │       │   │   ├── before.cpython-311.pyc
    │   │       │   │       │   │   ├── before_sleep.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── nap.cpython-311.pyc
    │   │       │   │       │   │   ├── retry.cpython-311.pyc
    │   │       │   │       │   │   ├── stop.cpython-311.pyc
    │   │       │   │       │   │   ├── tornadoweb.cpython-311.pyc
    │   │       │   │       │   │   ├── _utils.cpython-311.pyc
    │   │       │   │       │   │   └── wait.cpython-311.pyc
    │   │       │   │       │   ├── retry.py
    │   │       │   │       │   ├── stop.py
    │   │       │   │       │   ├── tornadoweb.py
    │   │       │   │       │   ├── _utils.py
    │   │       │   │       │   └── wait.py
    │   │       │   │       ├── tomli
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _parser.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _parser.cpython-311.pyc
    │   │       │   │       │   │   ├── _re.cpython-311.pyc
    │   │       │   │       │   │   └── _types.cpython-311.pyc
    │   │       │   │       │   ├── _re.py
    │   │       │   │       │   └── _types.py
    │   │       │   │       ├── typing_extensions.py
    │   │       │   │       ├── urllib3
    │   │       │   │       │   ├── _collections.py
    │   │       │   │       │   ├── connectionpool.py
    │   │       │   │       │   ├── connection.py
    │   │       │   │       │   ├── contrib
    │   │       │   │       │   │   ├── _appengine_environ.py
    │   │       │   │       │   │   ├── appengine.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── ntlmpool.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── appengine.cpython-311.pyc
    │   │       │   │       │   │   │   ├── _appengine_environ.cpython-311.pyc
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   ├── ntlmpool.cpython-311.pyc
    │   │       │   │       │   │   │   ├── pyopenssl.cpython-311.pyc
    │   │       │   │       │   │   │   ├── securetransport.cpython-311.pyc
    │   │       │   │       │   │   │   └── socks.cpython-311.pyc
    │   │       │   │       │   │   ├── pyopenssl.py
    │   │       │   │       │   │   ├── _securetransport
    │   │       │   │       │   │   │   ├── bindings.py
    │   │       │   │       │   │   │   ├── __init__.py
    │   │       │   │       │   │   │   ├── low_level.py
    │   │       │   │       │   │   │   └── __pycache__
    │   │       │   │       │   │   │       ├── bindings.cpython-311.pyc
    │   │       │   │       │   │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │       └── low_level.cpython-311.pyc
    │   │       │   │       │   │   ├── securetransport.py
    │   │       │   │       │   │   └── socks.py
    │   │       │   │       │   ├── exceptions.py
    │   │       │   │       │   ├── fields.py
    │   │       │   │       │   ├── filepost.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── packages
    │   │       │   │       │   │   ├── backports
    │   │       │   │       │   │   │   ├── __init__.py
    │   │       │   │       │   │   │   ├── makefile.py
    │   │       │   │       │   │   │   └── __pycache__
    │   │       │   │       │   │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │       └── makefile.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   └── six.cpython-311.pyc
    │   │       │   │       │   │   └── six.py
    │   │       │   │       │   ├── poolmanager.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── _collections.cpython-311.pyc
    │   │       │   │       │   │   ├── connection.cpython-311.pyc
    │   │       │   │       │   │   ├── connectionpool.cpython-311.pyc
    │   │       │   │       │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │       │   │   ├── fields.cpython-311.pyc
    │   │       │   │       │   │   ├── filepost.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── poolmanager.cpython-311.pyc
    │   │       │   │       │   │   ├── request.cpython-311.pyc
    │   │       │   │       │   │   ├── response.cpython-311.pyc
    │   │       │   │       │   │   └── _version.cpython-311.pyc
    │   │       │   │       │   ├── request.py
    │   │       │   │       │   ├── response.py
    │   │       │   │       │   ├── util
    │   │       │   │       │   │   ├── connection.py
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   ├── proxy.py
    │   │       │   │       │   │   ├── __pycache__
    │   │       │   │       │   │   │   ├── connection.cpython-311.pyc
    │   │       │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   │   ├── proxy.cpython-311.pyc
    │   │       │   │       │   │   │   ├── queue.cpython-311.pyc
    │   │       │   │       │   │   │   ├── request.cpython-311.pyc
    │   │       │   │       │   │   │   ├── response.cpython-311.pyc
    │   │       │   │       │   │   │   ├── retry.cpython-311.pyc
    │   │       │   │       │   │   │   ├── ssl_.cpython-311.pyc
    │   │       │   │       │   │   │   ├── ssl_match_hostname.cpython-311.pyc
    │   │       │   │       │   │   │   ├── ssltransport.cpython-311.pyc
    │   │       │   │       │   │   │   ├── timeout.cpython-311.pyc
    │   │       │   │       │   │   │   ├── url.cpython-311.pyc
    │   │       │   │       │   │   │   └── wait.cpython-311.pyc
    │   │       │   │       │   │   ├── queue.py
    │   │       │   │       │   │   ├── request.py
    │   │       │   │       │   │   ├── response.py
    │   │       │   │       │   │   ├── retry.py
    │   │       │   │       │   │   ├── ssl_match_hostname.py
    │   │       │   │       │   │   ├── ssl_.py
    │   │       │   │       │   │   ├── ssltransport.py
    │   │       │   │       │   │   ├── timeout.py
    │   │       │   │       │   │   ├── url.py
    │   │       │   │       │   │   └── wait.py
    │   │       │   │       │   └── _version.py
    │   │       │   │       ├── vendor.txt
    │   │       │   │       └── webencodings
    │   │       │   │           ├── __init__.py
    │   │       │   │           ├── labels.py
    │   │       │   │           ├── mklabels.py
    │   │       │   │           ├── __pycache__
    │   │       │   │           │   ├── __init__.cpython-311.pyc
    │   │       │   │           │   ├── labels.cpython-311.pyc
    │   │       │   │           │   ├── mklabels.cpython-311.pyc
    │   │       │   │           │   ├── tests.cpython-311.pyc
    │   │       │   │           │   └── x_user_defined.cpython-311.pyc
    │   │       │   │           ├── tests.py
    │   │       │   │           └── x_user_defined.py
    │   │       │   ├── pip-23.1.2.dist-info
    │   │       │   │   ├── AUTHORS.txt
    │   │       │   │   ├── entry_points.txt
    │   │       │   │   ├── INSTALLER
    │   │       │   │   ├── LICENSE.txt
    │   │       │   │   ├── METADATA
    │   │       │   │   ├── RECORD
    │   │       │   │   ├── REQUESTED
    │   │       │   │   ├── top_level.txt
    │   │       │   │   └── WHEEL
    │   │       │   ├── pkg_resources
    │   │       │   │   ├── extern
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   └── __pycache__
    │   │       │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   └── _vendor
    │   │       │   │       ├── appdirs.py
    │   │       │   │       ├── importlib_resources
    │   │       │   │       │   ├── abc.py
    │   │       │   │       │   ├── _adapters.py
    │   │       │   │       │   ├── _common.py
    │   │       │   │       │   ├── _compat.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _itertools.py
    │   │       │   │       │   ├── _legacy.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── abc.cpython-311.pyc
    │   │       │   │       │   │   ├── _adapters.cpython-311.pyc
    │   │       │   │       │   │   ├── _common.cpython-311.pyc
    │   │       │   │       │   │   ├── _compat.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │       │   │   ├── _legacy.cpython-311.pyc
    │   │       │   │       │   │   ├── readers.cpython-311.pyc
    │   │       │   │       │   │   └── simple.cpython-311.pyc
    │   │       │   │       │   ├── readers.py
    │   │       │   │       │   └── simple.py
    │   │       │   │       ├── __init__.py
    │   │       │   │       ├── jaraco
    │   │       │   │       │   ├── context.py
    │   │       │   │       │   ├── functools.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── context.cpython-311.pyc
    │   │       │   │       │   │   ├── functools.cpython-311.pyc
    │   │       │   │       │   │   └── __init__.cpython-311.pyc
    │   │       │   │       │   └── text
    │   │       │   │       │       ├── __init__.py
    │   │       │   │       │       └── __pycache__
    │   │       │   │       │           └── __init__.cpython-311.pyc
    │   │       │   │       ├── more_itertools
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── more.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── more.cpython-311.pyc
    │   │       │   │       │   │   └── recipes.cpython-311.pyc
    │   │       │   │       │   └── recipes.py
    │   │       │   │       ├── packaging
    │   │       │   │       │   ├── __about__.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── _manylinux.py
    │   │       │   │       │   ├── markers.py
    │   │       │   │       │   ├── _musllinux.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── __about__.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── _manylinux.cpython-311.pyc
    │   │       │   │       │   │   ├── markers.cpython-311.pyc
    │   │       │   │       │   │   ├── _musllinux.cpython-311.pyc
    │   │       │   │       │   │   ├── requirements.cpython-311.pyc
    │   │       │   │       │   │   ├── specifiers.cpython-311.pyc
    │   │       │   │       │   │   ├── _structures.cpython-311.pyc
    │   │       │   │       │   │   ├── tags.cpython-311.pyc
    │   │       │   │       │   │   ├── utils.cpython-311.pyc
    │   │       │   │       │   │   └── version.cpython-311.pyc
    │   │       │   │       │   ├── requirements.py
    │   │       │   │       │   ├── specifiers.py
    │   │       │   │       │   ├── _structures.py
    │   │       │   │       │   ├── tags.py
    │   │       │   │       │   ├── utils.py
    │   │       │   │       │   └── version.py
    │   │       │   │       ├── __pycache__
    │   │       │   │       │   ├── appdirs.cpython-311.pyc
    │   │       │   │       │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   └── zipp.cpython-311.pyc
    │   │       │   │       ├── pyparsing
    │   │       │   │       │   ├── actions.py
    │   │       │   │       │   ├── common.py
    │   │       │   │       │   ├── core.py
    │   │       │   │       │   ├── diagram
    │   │       │   │       │   │   ├── __init__.py
    │   │       │   │       │   │   └── __pycache__
    │   │       │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   │       │   ├── exceptions.py
    │   │       │   │       │   ├── helpers.py
    │   │       │   │       │   ├── __init__.py
    │   │       │   │       │   ├── __pycache__
    │   │       │   │       │   │   ├── actions.cpython-311.pyc
    │   │       │   │       │   │   ├── common.cpython-311.pyc
    │   │       │   │       │   │   ├── core.cpython-311.pyc
    │   │       │   │       │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │       │   │   ├── helpers.cpython-311.pyc
    │   │       │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │       │   │   ├── results.cpython-311.pyc
    │   │       │   │       │   │   ├── testing.cpython-311.pyc
    │   │       │   │       │   │   ├── unicode.cpython-311.pyc
    │   │       │   │       │   │   └── util.cpython-311.pyc
    │   │       │   │       │   ├── results.py
    │   │       │   │       │   ├── testing.py
    │   │       │   │       │   ├── unicode.py
    │   │       │   │       │   └── util.py
    │   │       │   │       └── zipp.py
    │   │       │   ├── README.txt
    │   │       │   ├── setuptools
    │   │       │   │   ├── archive_util.py
    │   │       │   │   ├── build_meta.py
    │   │       │   │   ├── cli-32.exe
    │   │       │   │   ├── cli-64.exe
    │   │       │   │   ├── cli-arm64.exe
    │   │       │   │   ├── cli.exe
    │   │       │   │   ├── command
    │   │       │   │   │   ├── alias.py
    │   │       │   │   │   ├── bdist_egg.py
    │   │       │   │   │   ├── bdist_rpm.py
    │   │       │   │   │   ├── build_clib.py
    │   │       │   │   │   ├── build_ext.py
    │   │       │   │   │   ├── build.py
    │   │       │   │   │   ├── build_py.py
    │   │       │   │   │   ├── develop.py
    │   │       │   │   │   ├── dist_info.py
    │   │       │   │   │   ├── easy_install.py
    │   │       │   │   │   ├── editable_wheel.py
    │   │       │   │   │   ├── egg_info.py
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── install_egg_info.py
    │   │       │   │   │   ├── install_lib.py
    │   │       │   │   │   ├── install.py
    │   │       │   │   │   ├── install_scripts.py
    │   │       │   │   │   ├── launcher manifest.xml
    │   │       │   │   │   ├── py36compat.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── alias.cpython-311.pyc
    │   │       │   │   │   │   ├── bdist_egg.cpython-311.pyc
    │   │       │   │   │   │   ├── bdist_rpm.cpython-311.pyc
    │   │       │   │   │   │   ├── build_clib.cpython-311.pyc
    │   │       │   │   │   │   ├── build.cpython-311.pyc
    │   │       │   │   │   │   ├── build_ext.cpython-311.pyc
    │   │       │   │   │   │   ├── build_py.cpython-311.pyc
    │   │       │   │   │   │   ├── develop.cpython-311.pyc
    │   │       │   │   │   │   ├── dist_info.cpython-311.pyc
    │   │       │   │   │   │   ├── easy_install.cpython-311.pyc
    │   │       │   │   │   │   ├── editable_wheel.cpython-311.pyc
    │   │       │   │   │   │   ├── egg_info.cpython-311.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── install.cpython-311.pyc
    │   │       │   │   │   │   ├── install_egg_info.cpython-311.pyc
    │   │       │   │   │   │   ├── install_lib.cpython-311.pyc
    │   │       │   │   │   │   ├── install_scripts.cpython-311.pyc
    │   │       │   │   │   │   ├── py36compat.cpython-311.pyc
    │   │       │   │   │   │   ├── register.cpython-311.pyc
    │   │       │   │   │   │   ├── rotate.cpython-311.pyc
    │   │       │   │   │   │   ├── saveopts.cpython-311.pyc
    │   │       │   │   │   │   ├── sdist.cpython-311.pyc
    │   │       │   │   │   │   ├── setopt.cpython-311.pyc
    │   │       │   │   │   │   ├── test.cpython-311.pyc
    │   │       │   │   │   │   ├── upload.cpython-311.pyc
    │   │       │   │   │   │   └── upload_docs.cpython-311.pyc
    │   │       │   │   │   ├── register.py
    │   │       │   │   │   ├── rotate.py
    │   │       │   │   │   ├── saveopts.py
    │   │       │   │   │   ├── sdist.py
    │   │       │   │   │   ├── setopt.py
    │   │       │   │   │   ├── test.py
    │   │       │   │   │   ├── upload_docs.py
    │   │       │   │   │   └── upload.py
    │   │       │   │   ├── config
    │   │       │   │   │   ├── _apply_pyprojecttoml.py
    │   │       │   │   │   ├── expand.py
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── _apply_pyprojecttoml.cpython-311.pyc
    │   │       │   │   │   │   ├── expand.cpython-311.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── pyprojecttoml.cpython-311.pyc
    │   │       │   │   │   │   └── setupcfg.cpython-311.pyc
    │   │       │   │   │   ├── pyprojecttoml.py
    │   │       │   │   │   ├── setupcfg.py
    │   │       │   │   │   └── _validate_pyproject
    │   │       │   │   │       ├── error_reporting.py
    │   │       │   │   │       ├── extra_validations.py
    │   │       │   │   │       ├── fastjsonschema_exceptions.py
    │   │       │   │   │       ├── fastjsonschema_validations.py
    │   │       │   │   │       ├── formats.py
    │   │       │   │   │       ├── __init__.py
    │   │       │   │   │       └── __pycache__
    │   │       │   │   │           ├── error_reporting.cpython-311.pyc
    │   │       │   │   │           ├── extra_validations.cpython-311.pyc
    │   │       │   │   │           ├── fastjsonschema_exceptions.cpython-311.pyc
    │   │       │   │   │           ├── fastjsonschema_validations.cpython-311.pyc
    │   │       │   │   │           ├── formats.cpython-311.pyc
    │   │       │   │   │           └── __init__.cpython-311.pyc
    │   │       │   │   ├── depends.py
    │   │       │   │   ├── _deprecation_warning.py
    │   │       │   │   ├── dep_util.py
    │   │       │   │   ├── discovery.py
    │   │       │   │   ├── dist.py
    │   │       │   │   ├── _distutils
    │   │       │   │   │   ├── archive_util.py
    │   │       │   │   │   ├── bcppcompiler.py
    │   │       │   │   │   ├── ccompiler.py
    │   │       │   │   │   ├── cmd.py
    │   │       │   │   │   ├── _collections.py
    │   │       │   │   │   ├── command
    │   │       │   │   │   │   ├── bdist_dumb.py
    │   │       │   │   │   │   ├── bdist.py
    │   │       │   │   │   │   ├── bdist_rpm.py
    │   │       │   │   │   │   ├── build_clib.py
    │   │       │   │   │   │   ├── build_ext.py
    │   │       │   │   │   │   ├── build.py
    │   │       │   │   │   │   ├── build_py.py
    │   │       │   │   │   │   ├── build_scripts.py
    │   │       │   │   │   │   ├── check.py
    │   │       │   │   │   │   ├── clean.py
    │   │       │   │   │   │   ├── config.py
    │   │       │   │   │   │   ├── _framework_compat.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── install_data.py
    │   │       │   │   │   │   ├── install_egg_info.py
    │   │       │   │   │   │   ├── install_headers.py
    │   │       │   │   │   │   ├── install_lib.py
    │   │       │   │   │   │   ├── install.py
    │   │       │   │   │   │   ├── install_scripts.py
    │   │       │   │   │   │   ├── py37compat.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── bdist.cpython-311.pyc
    │   │       │   │   │   │   │   ├── bdist_dumb.cpython-311.pyc
    │   │       │   │   │   │   │   ├── bdist_rpm.cpython-311.pyc
    │   │       │   │   │   │   │   ├── build_clib.cpython-311.pyc
    │   │       │   │   │   │   │   ├── build.cpython-311.pyc
    │   │       │   │   │   │   │   ├── build_ext.cpython-311.pyc
    │   │       │   │   │   │   │   ├── build_py.cpython-311.pyc
    │   │       │   │   │   │   │   ├── build_scripts.cpython-311.pyc
    │   │       │   │   │   │   │   ├── check.cpython-311.pyc
    │   │       │   │   │   │   │   ├── clean.cpython-311.pyc
    │   │       │   │   │   │   │   ├── config.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _framework_compat.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install_data.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install_egg_info.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install_headers.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install_lib.cpython-311.pyc
    │   │       │   │   │   │   │   ├── install_scripts.cpython-311.pyc
    │   │       │   │   │   │   │   ├── py37compat.cpython-311.pyc
    │   │       │   │   │   │   │   ├── register.cpython-311.pyc
    │   │       │   │   │   │   │   ├── sdist.cpython-311.pyc
    │   │       │   │   │   │   │   └── upload.cpython-311.pyc
    │   │       │   │   │   │   ├── register.py
    │   │       │   │   │   │   ├── sdist.py
    │   │       │   │   │   │   └── upload.py
    │   │       │   │   │   ├── config.py
    │   │       │   │   │   ├── core.py
    │   │       │   │   │   ├── cygwinccompiler.py
    │   │       │   │   │   ├── debug.py
    │   │       │   │   │   ├── dep_util.py
    │   │       │   │   │   ├── dir_util.py
    │   │       │   │   │   ├── dist.py
    │   │       │   │   │   ├── errors.py
    │   │       │   │   │   ├── extension.py
    │   │       │   │   │   ├── fancy_getopt.py
    │   │       │   │   │   ├── filelist.py
    │   │       │   │   │   ├── file_util.py
    │   │       │   │   │   ├── _functools.py
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── log.py
    │   │       │   │   │   ├── _macos_compat.py
    │   │       │   │   │   ├── msvc9compiler.py
    │   │       │   │   │   ├── _msvccompiler.py
    │   │       │   │   │   ├── msvccompiler.py
    │   │       │   │   │   ├── py38compat.py
    │   │       │   │   │   ├── py39compat.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── archive_util.cpython-311.pyc
    │   │       │   │   │   │   ├── bcppcompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── ccompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── cmd.cpython-311.pyc
    │   │       │   │   │   │   ├── _collections.cpython-311.pyc
    │   │       │   │   │   │   ├── config.cpython-311.pyc
    │   │       │   │   │   │   ├── core.cpython-311.pyc
    │   │       │   │   │   │   ├── cygwinccompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── debug.cpython-311.pyc
    │   │       │   │   │   │   ├── dep_util.cpython-311.pyc
    │   │       │   │   │   │   ├── dir_util.cpython-311.pyc
    │   │       │   │   │   │   ├── dist.cpython-311.pyc
    │   │       │   │   │   │   ├── errors.cpython-311.pyc
    │   │       │   │   │   │   ├── extension.cpython-311.pyc
    │   │       │   │   │   │   ├── fancy_getopt.cpython-311.pyc
    │   │       │   │   │   │   ├── filelist.cpython-311.pyc
    │   │       │   │   │   │   ├── file_util.cpython-311.pyc
    │   │       │   │   │   │   ├── _functools.cpython-311.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── log.cpython-311.pyc
    │   │       │   │   │   │   ├── _macos_compat.cpython-311.pyc
    │   │       │   │   │   │   ├── msvc9compiler.cpython-311.pyc
    │   │       │   │   │   │   ├── _msvccompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── msvccompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── py38compat.cpython-311.pyc
    │   │       │   │   │   │   ├── py39compat.cpython-311.pyc
    │   │       │   │   │   │   ├── spawn.cpython-311.pyc
    │   │       │   │   │   │   ├── sysconfig.cpython-311.pyc
    │   │       │   │   │   │   ├── text_file.cpython-311.pyc
    │   │       │   │   │   │   ├── unixccompiler.cpython-311.pyc
    │   │       │   │   │   │   ├── util.cpython-311.pyc
    │   │       │   │   │   │   ├── version.cpython-311.pyc
    │   │       │   │   │   │   └── versionpredicate.cpython-311.pyc
    │   │       │   │   │   ├── spawn.py
    │   │       │   │   │   ├── sysconfig.py
    │   │       │   │   │   ├── text_file.py
    │   │       │   │   │   ├── unixccompiler.py
    │   │       │   │   │   ├── util.py
    │   │       │   │   │   ├── versionpredicate.py
    │   │       │   │   │   └── version.py
    │   │       │   │   ├── _entry_points.py
    │   │       │   │   ├── errors.py
    │   │       │   │   ├── extension.py
    │   │       │   │   ├── extern
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   └── __pycache__
    │   │       │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   ├── glob.py
    │   │       │   │   ├── gui-32.exe
    │   │       │   │   ├── gui-64.exe
    │   │       │   │   ├── gui-arm64.exe
    │   │       │   │   ├── gui.exe
    │   │       │   │   ├── _importlib.py
    │   │       │   │   ├── _imp.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── installer.py
    │   │       │   │   ├── _itertools.py
    │   │       │   │   ├── launch.py
    │   │       │   │   ├── logging.py
    │   │       │   │   ├── monkey.py
    │   │       │   │   ├── msvc.py
    │   │       │   │   ├── namespaces.py
    │   │       │   │   ├── package_index.py
    │   │       │   │   ├── _path.py
    │   │       │   │   ├── py34compat.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── archive_util.cpython-311.pyc
    │   │       │   │   │   ├── build_meta.cpython-311.pyc
    │   │       │   │   │   ├── depends.cpython-311.pyc
    │   │       │   │   │   ├── _deprecation_warning.cpython-311.pyc
    │   │       │   │   │   ├── dep_util.cpython-311.pyc
    │   │       │   │   │   ├── discovery.cpython-311.pyc
    │   │       │   │   │   ├── dist.cpython-311.pyc
    │   │       │   │   │   ├── _entry_points.cpython-311.pyc
    │   │       │   │   │   ├── errors.cpython-311.pyc
    │   │       │   │   │   ├── extension.cpython-311.pyc
    │   │       │   │   │   ├── glob.cpython-311.pyc
    │   │       │   │   │   ├── _imp.cpython-311.pyc
    │   │       │   │   │   ├── _importlib.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── installer.cpython-311.pyc
    │   │       │   │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │   │   ├── launch.cpython-311.pyc
    │   │       │   │   │   ├── logging.cpython-311.pyc
    │   │       │   │   │   ├── monkey.cpython-311.pyc
    │   │       │   │   │   ├── msvc.cpython-311.pyc
    │   │       │   │   │   ├── namespaces.cpython-311.pyc
    │   │       │   │   │   ├── package_index.cpython-311.pyc
    │   │       │   │   │   ├── _path.cpython-311.pyc
    │   │       │   │   │   ├── py34compat.cpython-311.pyc
    │   │       │   │   │   ├── _reqs.cpython-311.pyc
    │   │       │   │   │   ├── sandbox.cpython-311.pyc
    │   │       │   │   │   ├── unicode_utils.cpython-311.pyc
    │   │       │   │   │   ├── version.cpython-311.pyc
    │   │       │   │   │   ├── wheel.cpython-311.pyc
    │   │       │   │   │   └── windows_support.cpython-311.pyc
    │   │       │   │   ├── _reqs.py
    │   │       │   │   ├── sandbox.py
    │   │       │   │   ├── script (dev).tmpl
    │   │       │   │   ├── script.tmpl
    │   │       │   │   ├── unicode_utils.py
    │   │       │   │   ├── _vendor
    │   │       │   │   │   ├── importlib_metadata
    │   │       │   │   │   │   ├── _adapters.py
    │   │       │   │   │   │   ├── _collections.py
    │   │       │   │   │   │   ├── _compat.py
    │   │       │   │   │   │   ├── _functools.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── _itertools.py
    │   │       │   │   │   │   ├── _meta.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── _adapters.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _collections.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _compat.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _functools.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _meta.cpython-311.pyc
    │   │       │   │   │   │   │   └── _text.cpython-311.pyc
    │   │       │   │   │   │   └── _text.py
    │   │       │   │   │   ├── importlib_resources
    │   │       │   │   │   │   ├── abc.py
    │   │       │   │   │   │   ├── _adapters.py
    │   │       │   │   │   │   ├── _common.py
    │   │       │   │   │   │   ├── _compat.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── _itertools.py
    │   │       │   │   │   │   ├── _legacy.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── abc.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _adapters.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _common.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _compat.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _itertools.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _legacy.cpython-311.pyc
    │   │       │   │   │   │   │   ├── readers.cpython-311.pyc
    │   │       │   │   │   │   │   └── simple.cpython-311.pyc
    │   │       │   │   │   │   ├── readers.py
    │   │       │   │   │   │   └── simple.py
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── jaraco
    │   │       │   │   │   │   ├── context.py
    │   │       │   │   │   │   ├── functools.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── context.cpython-311.pyc
    │   │       │   │   │   │   │   ├── functools.cpython-311.pyc
    │   │       │   │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   │   └── text
    │   │       │   │   │   │       ├── __init__.py
    │   │       │   │   │   │       └── __pycache__
    │   │       │   │   │   │           └── __init__.cpython-311.pyc
    │   │       │   │   │   ├── more_itertools
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── more.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── more.cpython-311.pyc
    │   │       │   │   │   │   │   └── recipes.cpython-311.pyc
    │   │       │   │   │   │   └── recipes.py
    │   │       │   │   │   ├── ordered_set.py
    │   │       │   │   │   ├── packaging
    │   │       │   │   │   │   ├── __about__.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── _manylinux.py
    │   │       │   │   │   │   ├── markers.py
    │   │       │   │   │   │   ├── _musllinux.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── __about__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _manylinux.cpython-311.pyc
    │   │       │   │   │   │   │   ├── markers.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _musllinux.cpython-311.pyc
    │   │       │   │   │   │   │   ├── requirements.cpython-311.pyc
    │   │       │   │   │   │   │   ├── specifiers.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _structures.cpython-311.pyc
    │   │       │   │   │   │   │   ├── tags.cpython-311.pyc
    │   │       │   │   │   │   │   ├── utils.cpython-311.pyc
    │   │       │   │   │   │   │   └── version.cpython-311.pyc
    │   │       │   │   │   │   ├── requirements.py
    │   │       │   │   │   │   ├── specifiers.py
    │   │       │   │   │   │   ├── _structures.py
    │   │       │   │   │   │   ├── tags.py
    │   │       │   │   │   │   ├── utils.py
    │   │       │   │   │   │   └── version.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── ordered_set.cpython-311.pyc
    │   │       │   │   │   │   ├── typing_extensions.cpython-311.pyc
    │   │       │   │   │   │   └── zipp.cpython-311.pyc
    │   │       │   │   │   ├── pyparsing
    │   │       │   │   │   │   ├── actions.py
    │   │       │   │   │   │   ├── common.py
    │   │       │   │   │   │   ├── core.py
    │   │       │   │   │   │   ├── diagram
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── exceptions.py
    │   │       │   │   │   │   ├── helpers.py
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── actions.cpython-311.pyc
    │   │       │   │   │   │   │   ├── common.cpython-311.pyc
    │   │       │   │   │   │   │   ├── core.cpython-311.pyc
    │   │       │   │   │   │   │   ├── exceptions.cpython-311.pyc
    │   │       │   │   │   │   │   ├── helpers.cpython-311.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── results.cpython-311.pyc
    │   │       │   │   │   │   │   ├── testing.cpython-311.pyc
    │   │       │   │   │   │   │   ├── unicode.cpython-311.pyc
    │   │       │   │   │   │   │   └── util.cpython-311.pyc
    │   │       │   │   │   │   ├── results.py
    │   │       │   │   │   │   ├── testing.py
    │   │       │   │   │   │   ├── unicode.py
    │   │       │   │   │   │   └── util.py
    │   │       │   │   │   ├── tomli
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── _parser.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _parser.cpython-311.pyc
    │   │       │   │   │   │   │   ├── _re.cpython-311.pyc
    │   │       │   │   │   │   │   └── _types.cpython-311.pyc
    │   │       │   │   │   │   ├── _re.py
    │   │       │   │   │   │   └── _types.py
    │   │       │   │   │   ├── typing_extensions.py
    │   │       │   │   │   └── zipp.py
    │   │       │   │   ├── version.py
    │   │       │   │   ├── wheel.py
    │   │       │   │   └── windows_support.py
    │   │       │   └── setuptools-65.5.0.dist-info
    │   │       │       ├── entry_points.txt
    │   │       │       ├── INSTALLER
    │   │       │       ├── LICENSE
    │   │       │       ├── METADATA
    │   │       │       ├── RECORD
    │   │       │       ├── REQUESTED
    │   │       │       ├── top_level.txt
    │   │       │       └── WHEEL
    │   │       ├── site.py
    │   │       ├── smtpd.py
    │   │       ├── smtplib.py
    │   │       ├── sndhdr.py
    │   │       ├── socket.py
    │   │       ├── socketserver.py
    │   │       ├── sqlite3
    │   │       │   ├── dbapi2.py
    │   │       │   ├── dump.py
    │   │       │   ├── __init__.py
    │   │       │   └── __pycache__
    │   │       │       ├── dbapi2.cpython-311.opt-1.pyc
    │   │       │       ├── dbapi2.cpython-311.opt-2.pyc
    │   │       │       ├── dbapi2.cpython-311.pyc
    │   │       │       ├── dump.cpython-311.opt-1.pyc
    │   │       │       ├── dump.cpython-311.opt-2.pyc
    │   │       │       ├── dump.cpython-311.pyc
    │   │       │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │       └── __init__.cpython-311.pyc
    │   │       ├── sre_compile.py
    │   │       ├── sre_constants.py
    │   │       ├── sre_parse.py
    │   │       ├── ssl.py
    │   │       ├── statistics.py
    │   │       ├── stat.py
    │   │       ├── stringprep.py
    │   │       ├── string.py
    │   │       ├── _strptime.py
    │   │       ├── struct.py
    │   │       ├── subprocess.py
    │   │       ├── sunau.py
    │   │       ├── symtable.py
    │   │       ├── _sysconfigdata__linux_x86_64-linux-gnu.py
    │   │       ├── sysconfig.py
    │   │       ├── tabnanny.py
    │   │       ├── tarfile.py
    │   │       ├── telnetlib.py
    │   │       ├── tempfile.py
    │   │       ├── test
    │   │       │   ├── allsans.pem
    │   │       │   ├── ann_module2.py
    │   │       │   ├── ann_module3.py
    │   │       │   ├── ann_module4.py
    │   │       │   ├── ann_module5.py
    │   │       │   ├── ann_module6.py
    │   │       │   ├── ann_module7.py
    │   │       │   ├── ann_module8.py
    │   │       │   ├── ann_module.py
    │   │       │   ├── audiodata
    │   │       │   │   ├── pluck-alaw.aifc
    │   │       │   │   ├── pluck-pcm16.aiff
    │   │       │   │   ├── pluck-pcm16.au
    │   │       │   │   ├── pluck-pcm16.wav
    │   │       │   │   ├── pluck-pcm24.aiff
    │   │       │   │   ├── pluck-pcm24.au
    │   │       │   │   ├── pluck-pcm24.wav
    │   │       │   │   ├── pluck-pcm32.aiff
    │   │       │   │   ├── pluck-pcm32.au
    │   │       │   │   ├── pluck-pcm32.wav
    │   │       │   │   ├── pluck-pcm8.aiff
    │   │       │   │   ├── pluck-pcm8.au
    │   │       │   │   ├── pluck-pcm8.wav
    │   │       │   │   ├── pluck-ulaw.aifc
    │   │       │   │   └── pluck-ulaw.au
    │   │       │   ├── audiotest.au
    │   │       │   ├── audiotests.py
    │   │       │   ├── audit-tests.py
    │   │       │   ├── autotest.py
    │   │       │   ├── badcert.pem
    │   │       │   ├── bad_coding2.py
    │   │       │   ├── bad_coding.py
    │   │       │   ├── bad_getattr2.py
    │   │       │   ├── bad_getattr3.py
    │   │       │   ├── bad_getattr.py
    │   │       │   ├── badkey.pem
    │   │       │   ├── badsyntax_3131.py
    │   │       │   ├── badsyntax_future10.py
    │   │       │   ├── badsyntax_future3.py
    │   │       │   ├── badsyntax_future4.py
    │   │       │   ├── badsyntax_future5.py
    │   │       │   ├── badsyntax_future6.py
    │   │       │   ├── badsyntax_future7.py
    │   │       │   ├── badsyntax_future8.py
    │   │       │   ├── badsyntax_future9.py
    │   │       │   ├── badsyntax_pep3120.py
    │   │       │   ├── bisect_cmd.py
    │   │       │   ├── capath
    │   │       │   │   ├── 4e1295a3.0
    │   │       │   │   ├── 5ed36f99.0
    │   │       │   │   ├── 6e88d7b8.0
    │   │       │   │   ├── 99d0fa06.0
    │   │       │   │   ├── b1930218.0
    │   │       │   │   └── ceff1710.0
    │   │       │   ├── cfgparser.1
    │   │       │   ├── cfgparser.2
    │   │       │   ├── cfgparser.3
    │   │       │   ├── cjkencodings
    │   │       │   │   ├── big5hkscs.txt
    │   │       │   │   ├── big5hkscs-utf8.txt
    │   │       │   │   ├── big5.txt
    │   │       │   │   ├── big5-utf8.txt
    │   │       │   │   ├── cp949.txt
    │   │       │   │   ├── cp949-utf8.txt
    │   │       │   │   ├── euc_jisx0213.txt
    │   │       │   │   ├── euc_jisx0213-utf8.txt
    │   │       │   │   ├── euc_jp.txt
    │   │       │   │   ├── euc_jp-utf8.txt
    │   │       │   │   ├── euc_kr.txt
    │   │       │   │   ├── euc_kr-utf8.txt
    │   │       │   │   ├── gb18030.txt
    │   │       │   │   ├── gb18030-utf8.txt
    │   │       │   │   ├── gb2312.txt
    │   │       │   │   ├── gb2312-utf8.txt
    │   │       │   │   ├── gbk.txt
    │   │       │   │   ├── gbk-utf8.txt
    │   │       │   │   ├── hz.txt
    │   │       │   │   ├── hz-utf8.txt
    │   │       │   │   ├── iso2022_jp.txt
    │   │       │   │   ├── iso2022_jp-utf8.txt
    │   │       │   │   ├── iso2022_kr.txt
    │   │       │   │   ├── iso2022_kr-utf8.txt
    │   │       │   │   ├── johab.txt
    │   │       │   │   ├── johab-utf8.txt
    │   │       │   │   ├── shift_jis.txt
    │   │       │   │   ├── shift_jis-utf8.txt
    │   │       │   │   ├── shift_jisx0213.txt
    │   │       │   │   └── shift_jisx0213-utf8.txt
    │   │       │   ├── clinic.test
    │   │       │   ├── cmath_testcases.txt
    │   │       │   ├── coding20731.py
    │   │       │   ├── crashers
    │   │       │   │   ├── bogus_code_obj.py
    │   │       │   │   ├── gc_inspection.py
    │   │       │   │   ├── infinite_loop_re.py
    │   │       │   │   ├── mutation_inside_cyclegc.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── bogus_code_obj.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── bogus_code_obj.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── bogus_code_obj.cpython-311.pyc
    │   │       │   │   │   ├── gc_inspection.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── gc_inspection.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── gc_inspection.cpython-311.pyc
    │   │       │   │   │   ├── infinite_loop_re.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── infinite_loop_re.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── infinite_loop_re.cpython-311.pyc
    │   │       │   │   │   ├── mutation_inside_cyclegc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── mutation_inside_cyclegc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── mutation_inside_cyclegc.cpython-311.pyc
    │   │       │   │   │   ├── recursive_call.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── recursive_call.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── recursive_call.cpython-311.pyc
    │   │       │   │   │   ├── trace_at_recursion_limit.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── trace_at_recursion_limit.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── trace_at_recursion_limit.cpython-311.pyc
    │   │       │   │   │   ├── underlying_dict.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── underlying_dict.cpython-311.opt-2.pyc
    │   │       │   │   │   └── underlying_dict.cpython-311.pyc
    │   │       │   │   ├── README
    │   │       │   │   ├── recursive_call.py
    │   │       │   │   ├── trace_at_recursion_limit.py
    │   │       │   │   └── underlying_dict.py
    │   │       │   ├── curses_tests.py
    │   │       │   ├── data
    │   │       │   │   └── README
    │   │       │   ├── dataclass_module_1.py
    │   │       │   ├── dataclass_module_1_str.py
    │   │       │   ├── dataclass_module_2.py
    │   │       │   ├── dataclass_module_2_str.py
    │   │       │   ├── dataclass_textanno.py
    │   │       │   ├── datetimetester.py
    │   │       │   ├── decimaltestdata
    │   │       │   │   ├── abs.decTest
    │   │       │   │   ├── add.decTest
    │   │       │   │   ├── and.decTest
    │   │       │   │   ├── base.decTest
    │   │       │   │   ├── clamp.decTest
    │   │       │   │   ├── class.decTest
    │   │       │   │   ├── compare.decTest
    │   │       │   │   ├── comparetotal.decTest
    │   │       │   │   ├── comparetotmag.decTest
    │   │       │   │   ├── copyabs.decTest
    │   │       │   │   ├── copy.decTest
    │   │       │   │   ├── copynegate.decTest
    │   │       │   │   ├── copysign.decTest
    │   │       │   │   ├── ddAbs.decTest
    │   │       │   │   ├── ddAdd.decTest
    │   │       │   │   ├── ddAnd.decTest
    │   │       │   │   ├── ddBase.decTest
    │   │       │   │   ├── ddCanonical.decTest
    │   │       │   │   ├── ddClass.decTest
    │   │       │   │   ├── ddCompare.decTest
    │   │       │   │   ├── ddCompareSig.decTest
    │   │       │   │   ├── ddCompareTotal.decTest
    │   │       │   │   ├── ddCompareTotalMag.decTest
    │   │       │   │   ├── ddCopyAbs.decTest
    │   │       │   │   ├── ddCopy.decTest
    │   │       │   │   ├── ddCopyNegate.decTest
    │   │       │   │   ├── ddCopySign.decTest
    │   │       │   │   ├── ddDivide.decTest
    │   │       │   │   ├── ddDivideInt.decTest
    │   │       │   │   ├── ddEncode.decTest
    │   │       │   │   ├── ddFMA.decTest
    │   │       │   │   ├── ddInvert.decTest
    │   │       │   │   ├── ddLogB.decTest
    │   │       │   │   ├── ddMax.decTest
    │   │       │   │   ├── ddMaxMag.decTest
    │   │       │   │   ├── ddMin.decTest
    │   │       │   │   ├── ddMinMag.decTest
    │   │       │   │   ├── ddMinus.decTest
    │   │       │   │   ├── ddMultiply.decTest
    │   │       │   │   ├── ddNextMinus.decTest
    │   │       │   │   ├── ddNextPlus.decTest
    │   │       │   │   ├── ddNextToward.decTest
    │   │       │   │   ├── ddOr.decTest
    │   │       │   │   ├── ddPlus.decTest
    │   │       │   │   ├── ddQuantize.decTest
    │   │       │   │   ├── ddReduce.decTest
    │   │       │   │   ├── ddRemainder.decTest
    │   │       │   │   ├── ddRemainderNear.decTest
    │   │       │   │   ├── ddRotate.decTest
    │   │       │   │   ├── ddSameQuantum.decTest
    │   │       │   │   ├── ddScaleB.decTest
    │   │       │   │   ├── ddShift.decTest
    │   │       │   │   ├── ddSubtract.decTest
    │   │       │   │   ├── ddToIntegral.decTest
    │   │       │   │   ├── ddXor.decTest
    │   │       │   │   ├── decDouble.decTest
    │   │       │   │   ├── decQuad.decTest
    │   │       │   │   ├── decSingle.decTest
    │   │       │   │   ├── divide.decTest
    │   │       │   │   ├── divideint.decTest
    │   │       │   │   ├── dqAbs.decTest
    │   │       │   │   ├── dqAdd.decTest
    │   │       │   │   ├── dqAnd.decTest
    │   │       │   │   ├── dqBase.decTest
    │   │       │   │   ├── dqCanonical.decTest
    │   │       │   │   ├── dqClass.decTest
    │   │       │   │   ├── dqCompare.decTest
    │   │       │   │   ├── dqCompareSig.decTest
    │   │       │   │   ├── dqCompareTotal.decTest
    │   │       │   │   ├── dqCompareTotalMag.decTest
    │   │       │   │   ├── dqCopyAbs.decTest
    │   │       │   │   ├── dqCopy.decTest
    │   │       │   │   ├── dqCopyNegate.decTest
    │   │       │   │   ├── dqCopySign.decTest
    │   │       │   │   ├── dqDivide.decTest
    │   │       │   │   ├── dqDivideInt.decTest
    │   │       │   │   ├── dqEncode.decTest
    │   │       │   │   ├── dqFMA.decTest
    │   │       │   │   ├── dqInvert.decTest
    │   │       │   │   ├── dqLogB.decTest
    │   │       │   │   ├── dqMax.decTest
    │   │       │   │   ├── dqMaxMag.decTest
    │   │       │   │   ├── dqMin.decTest
    │   │       │   │   ├── dqMinMag.decTest
    │   │       │   │   ├── dqMinus.decTest
    │   │       │   │   ├── dqMultiply.decTest
    │   │       │   │   ├── dqNextMinus.decTest
    │   │       │   │   ├── dqNextPlus.decTest
    │   │       │   │   ├── dqNextToward.decTest
    │   │       │   │   ├── dqOr.decTest
    │   │       │   │   ├── dqPlus.decTest
    │   │       │   │   ├── dqQuantize.decTest
    │   │       │   │   ├── dqReduce.decTest
    │   │       │   │   ├── dqRemainder.decTest
    │   │       │   │   ├── dqRemainderNear.decTest
    │   │       │   │   ├── dqRotate.decTest
    │   │       │   │   ├── dqSameQuantum.decTest
    │   │       │   │   ├── dqScaleB.decTest
    │   │       │   │   ├── dqShift.decTest
    │   │       │   │   ├── dqSubtract.decTest
    │   │       │   │   ├── dqToIntegral.decTest
    │   │       │   │   ├── dqXor.decTest
    │   │       │   │   ├── dsBase.decTest
    │   │       │   │   ├── dsEncode.decTest
    │   │       │   │   ├── exp.decTest
    │   │       │   │   ├── extra.decTest
    │   │       │   │   ├── fma.decTest
    │   │       │   │   ├── inexact.decTest
    │   │       │   │   ├── invert.decTest
    │   │       │   │   ├── ln.decTest
    │   │       │   │   ├── log10.decTest
    │   │       │   │   ├── logb.decTest
    │   │       │   │   ├── max.decTest
    │   │       │   │   ├── maxmag.decTest
    │   │       │   │   ├── min.decTest
    │   │       │   │   ├── minmag.decTest
    │   │       │   │   ├── minus.decTest
    │   │       │   │   ├── multiply.decTest
    │   │       │   │   ├── nextminus.decTest
    │   │       │   │   ├── nextplus.decTest
    │   │       │   │   ├── nexttoward.decTest
    │   │       │   │   ├── or.decTest
    │   │       │   │   ├── plus.decTest
    │   │       │   │   ├── power.decTest
    │   │       │   │   ├── powersqrt.decTest
    │   │       │   │   ├── quantize.decTest
    │   │       │   │   ├── randomBound32.decTest
    │   │       │   │   ├── randoms.decTest
    │   │       │   │   ├── reduce.decTest
    │   │       │   │   ├── remainder.decTest
    │   │       │   │   ├── remainderNear.decTest
    │   │       │   │   ├── rescale.decTest
    │   │       │   │   ├── rotate.decTest
    │   │       │   │   ├── rounding.decTest
    │   │       │   │   ├── samequantum.decTest
    │   │       │   │   ├── scaleb.decTest
    │   │       │   │   ├── shift.decTest
    │   │       │   │   ├── squareroot.decTest
    │   │       │   │   ├── subtract.decTest
    │   │       │   │   ├── testall.decTest
    │   │       │   │   ├── tointegral.decTest
    │   │       │   │   ├── tointegralx.decTest
    │   │       │   │   └── xor.decTest
    │   │       │   ├── dis_module.py
    │   │       │   ├── doctest_aliases.py
    │   │       │   ├── doctest_lineno.py
    │   │       │   ├── double_const.py
    │   │       │   ├── dtracedata
    │   │       │   │   ├── assert_usable.d
    │   │       │   │   ├── assert_usable.stp
    │   │       │   │   ├── call_stack.d
    │   │       │   │   ├── call_stack.d.expected
    │   │       │   │   ├── call_stack.py
    │   │       │   │   ├── call_stack.stp
    │   │       │   │   ├── call_stack.stp.expected
    │   │       │   │   ├── gc.d
    │   │       │   │   ├── gc.d.expected
    │   │       │   │   ├── gc.py
    │   │       │   │   ├── gc.stp
    │   │       │   │   ├── gc.stp.expected
    │   │       │   │   ├── instance.py
    │   │       │   │   ├── line.d
    │   │       │   │   ├── line.d.expected
    │   │       │   │   ├── line.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── call_stack.cpython-311.opt-1.pyc
    │   │       │   │       ├── call_stack.cpython-311.opt-2.pyc
    │   │       │   │       ├── call_stack.cpython-311.pyc
    │   │       │   │       ├── gc.cpython-311.opt-1.pyc
    │   │       │   │       ├── gc.cpython-311.opt-2.pyc
    │   │       │   │       ├── gc.cpython-311.pyc
    │   │       │   │       ├── instance.cpython-311.opt-1.pyc
    │   │       │   │       ├── instance.cpython-311.opt-2.pyc
    │   │       │   │       ├── instance.cpython-311.pyc
    │   │       │   │       ├── line.cpython-311.opt-1.pyc
    │   │       │   │       ├── line.cpython-311.opt-2.pyc
    │   │       │   │       └── line.cpython-311.pyc
    │   │       │   ├── empty.vbs
    │   │       │   ├── encoded_modules
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── module_iso_8859_1.py
    │   │       │   │   ├── module_koi8_r.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       ├── module_iso_8859_1.cpython-311.opt-1.pyc
    │   │       │   │       ├── module_iso_8859_1.cpython-311.opt-2.pyc
    │   │       │   │       ├── module_iso_8859_1.cpython-311.pyc
    │   │       │   │       ├── module_koi8_r.cpython-311.opt-1.pyc
    │   │       │   │       ├── module_koi8_r.cpython-311.opt-2.pyc
    │   │       │   │       └── module_koi8_r.cpython-311.pyc
    │   │       │   ├── exception_hierarchy.txt
    │   │       │   ├── ffdh3072.pem
    │   │       │   ├── final_a.py
    │   │       │   ├── final_b.py
    │   │       │   ├── floating_points.txt
    │   │       │   ├── fork_wait.py
    │   │       │   ├── formatfloat_testcases.txt
    │   │       │   ├── future_test1.py
    │   │       │   ├── future_test2.py
    │   │       │   ├── gdb_sample.py
    │   │       │   ├── good_getattr.py
    │   │       │   ├── idnsans.pem
    │   │       │   ├── ieee754.txt
    │   │       │   ├── imghdrdata
    │   │       │   │   ├── python.bmp
    │   │       │   │   ├── python.exr
    │   │       │   │   ├── python.gif
    │   │       │   │   ├── python.jpg
    │   │       │   │   ├── python.pbm
    │   │       │   │   ├── python.pgm
    │   │       │   │   ├── python.png
    │   │       │   │   ├── python.ppm
    │   │       │   │   ├── python.ras
    │   │       │   │   ├── python-raw.jpg
    │   │       │   │   ├── python.sgi
    │   │       │   │   ├── python.tiff
    │   │       │   │   ├── python.webp
    │   │       │   │   └── python.xbm
    │   │       │   ├── imp_dummy.py
    │   │       │   ├── __init__.py
    │   │       │   ├── inspect_fodder2.py
    │   │       │   ├── inspect_fodder.py
    │   │       │   ├── inspect_stock_annotations.py
    │   │       │   ├── inspect_stringized_annotations_2.py
    │   │       │   ├── inspect_stringized_annotations.py
    │   │       │   ├── keycert2.pem
    │   │       │   ├── keycert3.pem
    │   │       │   ├── keycert4.pem
    │   │       │   ├── keycertecc.pem
    │   │       │   ├── keycert.passwd.pem
    │   │       │   ├── keycert.pem
    │   │       │   ├── leakers
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── test_ctypes.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_ctypes.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_ctypes.cpython-311.pyc
    │   │       │   │   │   ├── test_selftype.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_selftype.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_selftype.cpython-311.pyc
    │   │       │   │   ├── README.txt
    │   │       │   │   ├── test_ctypes.py
    │   │       │   │   └── test_selftype.py
    │   │       │   ├── libregrtest
    │   │       │   │   ├── cmdline.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── main.py
    │   │       │   │   ├── pgo.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── cmdline.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── cmdline.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── cmdline.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── main.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── main.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── main.cpython-311.pyc
    │   │       │   │   │   ├── pgo.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── pgo.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── pgo.cpython-311.pyc
    │   │       │   │   │   ├── refleak.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── refleak.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── refleak.cpython-311.pyc
    │   │       │   │   │   ├── runtest.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── runtest.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── runtest.cpython-311.pyc
    │   │       │   │   │   ├── runtest_mp.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── runtest_mp.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── runtest_mp.cpython-311.pyc
    │   │       │   │   │   ├── save_env.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── save_env.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── save_env.cpython-311.pyc
    │   │       │   │   │   ├── setup.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── setup.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── setup.cpython-311.pyc
    │   │       │   │   │   ├── utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── utils.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── utils.cpython-311.pyc
    │   │       │   │   │   ├── win_utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── win_utils.cpython-311.opt-2.pyc
    │   │       │   │   │   └── win_utils.cpython-311.pyc
    │   │       │   │   ├── refleak.py
    │   │       │   │   ├── runtest_mp.py
    │   │       │   │   ├── runtest.py
    │   │       │   │   ├── save_env.py
    │   │       │   │   ├── setup.py
    │   │       │   │   ├── utils.py
    │   │       │   │   └── win_utils.py
    │   │       │   ├── list_tests.py
    │   │       │   ├── lock_tests.py
    │   │       │   ├── mailcap.txt
    │   │       │   ├── __main__.py
    │   │       │   ├── make_ssl_certs.py
    │   │       │   ├── mapping_tests.py
    │   │       │   ├── math_testcases.txt
    │   │       │   ├── memory_watchdog.py
    │   │       │   ├── mime.types
    │   │       │   ├── mock_socket.py
    │   │       │   ├── mod_generics_cache.py
    │   │       │   ├── mp_fork_bomb.py
    │   │       │   ├── mp_preload.py
    │   │       │   ├── multibytecodec_support.py
    │   │       │   ├── nokia.pem
    │   │       │   ├── nosan.pem
    │   │       │   ├── nullbytecert.pem
    │   │       │   ├── nullcert.pem
    │   │       │   ├── pickletester.py
    │   │       │   ├── profilee.py
    │   │       │   ├── pstats.pck
    │   │       │   ├── pycacert.pem
    │   │       │   ├── __pycache__
    │   │       │   │   ├── ann_module2.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module2.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module2.cpython-311.pyc
    │   │       │   │   ├── ann_module3.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module3.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module3.cpython-311.pyc
    │   │       │   │   ├── ann_module4.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module4.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module4.cpython-311.pyc
    │   │       │   │   ├── ann_module5.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module5.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module5.cpython-311.pyc
    │   │       │   │   ├── ann_module6.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module6.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module6.cpython-311.pyc
    │   │       │   │   ├── ann_module7.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module7.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module7.cpython-311.pyc
    │   │       │   │   ├── ann_module8.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module8.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module8.cpython-311.pyc
    │   │       │   │   ├── ann_module.cpython-311.opt-1.pyc
    │   │       │   │   ├── ann_module.cpython-311.opt-2.pyc
    │   │       │   │   ├── ann_module.cpython-311.pyc
    │   │       │   │   ├── audiotests.cpython-311.opt-1.pyc
    │   │       │   │   ├── audiotests.cpython-311.opt-2.pyc
    │   │       │   │   ├── audiotests.cpython-311.pyc
    │   │       │   │   ├── audit-tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── audit-tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── audit-tests.cpython-311.pyc
    │   │       │   │   ├── autotest.cpython-311.opt-1.pyc
    │   │       │   │   ├── autotest.cpython-311.opt-2.pyc
    │   │       │   │   ├── autotest.cpython-311.pyc
    │   │       │   │   ├── bad_getattr2.cpython-311.opt-1.pyc
    │   │       │   │   ├── bad_getattr2.cpython-311.opt-2.pyc
    │   │       │   │   ├── bad_getattr2.cpython-311.pyc
    │   │       │   │   ├── bad_getattr3.cpython-311.opt-1.pyc
    │   │       │   │   ├── bad_getattr3.cpython-311.opt-2.pyc
    │   │       │   │   ├── bad_getattr3.cpython-311.pyc
    │   │       │   │   ├── bad_getattr.cpython-311.opt-1.pyc
    │   │       │   │   ├── bad_getattr.cpython-311.opt-2.pyc
    │   │       │   │   ├── bad_getattr.cpython-311.pyc
    │   │       │   │   ├── bisect_cmd.cpython-311.opt-1.pyc
    │   │       │   │   ├── bisect_cmd.cpython-311.opt-2.pyc
    │   │       │   │   ├── bisect_cmd.cpython-311.pyc
    │   │       │   │   ├── coding20731.cpython-311.opt-1.pyc
    │   │       │   │   ├── coding20731.cpython-311.opt-2.pyc
    │   │       │   │   ├── coding20731.cpython-311.pyc
    │   │       │   │   ├── curses_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── curses_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── curses_tests.cpython-311.pyc
    │   │       │   │   ├── dataclass_module_1.cpython-311.opt-1.pyc
    │   │       │   │   ├── dataclass_module_1.cpython-311.opt-2.pyc
    │   │       │   │   ├── dataclass_module_1.cpython-311.pyc
    │   │       │   │   ├── dataclass_module_1_str.cpython-311.opt-1.pyc
    │   │       │   │   ├── dataclass_module_1_str.cpython-311.opt-2.pyc
    │   │       │   │   ├── dataclass_module_1_str.cpython-311.pyc
    │   │       │   │   ├── dataclass_module_2.cpython-311.opt-1.pyc
    │   │       │   │   ├── dataclass_module_2.cpython-311.opt-2.pyc
    │   │       │   │   ├── dataclass_module_2.cpython-311.pyc
    │   │       │   │   ├── dataclass_module_2_str.cpython-311.opt-1.pyc
    │   │       │   │   ├── dataclass_module_2_str.cpython-311.opt-2.pyc
    │   │       │   │   ├── dataclass_module_2_str.cpython-311.pyc
    │   │       │   │   ├── dataclass_textanno.cpython-311.opt-1.pyc
    │   │       │   │   ├── dataclass_textanno.cpython-311.opt-2.pyc
    │   │       │   │   ├── dataclass_textanno.cpython-311.pyc
    │   │       │   │   ├── datetimetester.cpython-311.opt-1.pyc
    │   │       │   │   ├── datetimetester.cpython-311.opt-2.pyc
    │   │       │   │   ├── datetimetester.cpython-311.pyc
    │   │       │   │   ├── dis_module.cpython-311.opt-1.pyc
    │   │       │   │   ├── dis_module.cpython-311.opt-2.pyc
    │   │       │   │   ├── dis_module.cpython-311.pyc
    │   │       │   │   ├── doctest_aliases.cpython-311.opt-1.pyc
    │   │       │   │   ├── doctest_aliases.cpython-311.opt-2.pyc
    │   │       │   │   ├── doctest_aliases.cpython-311.pyc
    │   │       │   │   ├── doctest_lineno.cpython-311.opt-1.pyc
    │   │       │   │   ├── doctest_lineno.cpython-311.opt-2.pyc
    │   │       │   │   ├── doctest_lineno.cpython-311.pyc
    │   │       │   │   ├── double_const.cpython-311.opt-1.pyc
    │   │       │   │   ├── double_const.cpython-311.opt-2.pyc
    │   │       │   │   ├── double_const.cpython-311.pyc
    │   │       │   │   ├── final_a.cpython-311.opt-1.pyc
    │   │       │   │   ├── final_a.cpython-311.opt-2.pyc
    │   │       │   │   ├── final_a.cpython-311.pyc
    │   │       │   │   ├── final_b.cpython-311.opt-1.pyc
    │   │       │   │   ├── final_b.cpython-311.opt-2.pyc
    │   │       │   │   ├── final_b.cpython-311.pyc
    │   │       │   │   ├── fork_wait.cpython-311.opt-1.pyc
    │   │       │   │   ├── fork_wait.cpython-311.opt-2.pyc
    │   │       │   │   ├── fork_wait.cpython-311.pyc
    │   │       │   │   ├── future_test1.cpython-311.opt-1.pyc
    │   │       │   │   ├── future_test1.cpython-311.opt-2.pyc
    │   │       │   │   ├── future_test1.cpython-311.pyc
    │   │       │   │   ├── future_test2.cpython-311.opt-1.pyc
    │   │       │   │   ├── future_test2.cpython-311.opt-2.pyc
    │   │       │   │   ├── future_test2.cpython-311.pyc
    │   │       │   │   ├── gdb_sample.cpython-311.opt-1.pyc
    │   │       │   │   ├── gdb_sample.cpython-311.opt-2.pyc
    │   │       │   │   ├── gdb_sample.cpython-311.pyc
    │   │       │   │   ├── good_getattr.cpython-311.opt-1.pyc
    │   │       │   │   ├── good_getattr.cpython-311.opt-2.pyc
    │   │       │   │   ├── good_getattr.cpython-311.pyc
    │   │       │   │   ├── imp_dummy.cpython-311.opt-1.pyc
    │   │       │   │   ├── imp_dummy.cpython-311.opt-2.pyc
    │   │       │   │   ├── imp_dummy.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── inspect_fodder2.cpython-311.opt-1.pyc
    │   │       │   │   ├── inspect_fodder2.cpython-311.opt-2.pyc
    │   │       │   │   ├── inspect_fodder2.cpython-311.pyc
    │   │       │   │   ├── inspect_fodder.cpython-311.opt-1.pyc
    │   │       │   │   ├── inspect_fodder.cpython-311.opt-2.pyc
    │   │       │   │   ├── inspect_fodder.cpython-311.pyc
    │   │       │   │   ├── inspect_stock_annotations.cpython-311.opt-1.pyc
    │   │       │   │   ├── inspect_stock_annotations.cpython-311.opt-2.pyc
    │   │       │   │   ├── inspect_stock_annotations.cpython-311.pyc
    │   │       │   │   ├── inspect_stringized_annotations_2.cpython-311.opt-1.pyc
    │   │       │   │   ├── inspect_stringized_annotations_2.cpython-311.opt-2.pyc
    │   │       │   │   ├── inspect_stringized_annotations_2.cpython-311.pyc
    │   │       │   │   ├── inspect_stringized_annotations.cpython-311.opt-1.pyc
    │   │       │   │   ├── inspect_stringized_annotations.cpython-311.opt-2.pyc
    │   │       │   │   ├── inspect_stringized_annotations.cpython-311.pyc
    │   │       │   │   ├── list_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── list_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── list_tests.cpython-311.pyc
    │   │       │   │   ├── lock_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── lock_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── lock_tests.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── make_ssl_certs.cpython-311.opt-1.pyc
    │   │       │   │   ├── make_ssl_certs.cpython-311.opt-2.pyc
    │   │       │   │   ├── make_ssl_certs.cpython-311.pyc
    │   │       │   │   ├── mapping_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── mapping_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── mapping_tests.cpython-311.pyc
    │   │       │   │   ├── memory_watchdog.cpython-311.opt-1.pyc
    │   │       │   │   ├── memory_watchdog.cpython-311.opt-2.pyc
    │   │       │   │   ├── memory_watchdog.cpython-311.pyc
    │   │       │   │   ├── mock_socket.cpython-311.opt-1.pyc
    │   │       │   │   ├── mock_socket.cpython-311.opt-2.pyc
    │   │       │   │   ├── mock_socket.cpython-311.pyc
    │   │       │   │   ├── mod_generics_cache.cpython-311.opt-1.pyc
    │   │       │   │   ├── mod_generics_cache.cpython-311.opt-2.pyc
    │   │       │   │   ├── mod_generics_cache.cpython-311.pyc
    │   │       │   │   ├── mp_fork_bomb.cpython-311.opt-1.pyc
    │   │       │   │   ├── mp_fork_bomb.cpython-311.opt-2.pyc
    │   │       │   │   ├── mp_fork_bomb.cpython-311.pyc
    │   │       │   │   ├── mp_preload.cpython-311.opt-1.pyc
    │   │       │   │   ├── mp_preload.cpython-311.opt-2.pyc
    │   │       │   │   ├── mp_preload.cpython-311.pyc
    │   │       │   │   ├── multibytecodec_support.cpython-311.opt-1.pyc
    │   │       │   │   ├── multibytecodec_support.cpython-311.opt-2.pyc
    │   │       │   │   ├── multibytecodec_support.cpython-311.pyc
    │   │       │   │   ├── pickletester.cpython-311.opt-1.pyc
    │   │       │   │   ├── pickletester.cpython-311.opt-2.pyc
    │   │       │   │   ├── pickletester.cpython-311.pyc
    │   │       │   │   ├── profilee.cpython-311.opt-1.pyc
    │   │       │   │   ├── profilee.cpython-311.opt-2.pyc
    │   │       │   │   ├── profilee.cpython-311.pyc
    │   │       │   │   ├── pyclbr_input.cpython-311.opt-1.pyc
    │   │       │   │   ├── pyclbr_input.cpython-311.opt-2.pyc
    │   │       │   │   ├── pyclbr_input.cpython-311.pyc
    │   │       │   │   ├── pydocfodder.cpython-311.opt-1.pyc
    │   │       │   │   ├── pydocfodder.cpython-311.opt-2.pyc
    │   │       │   │   ├── pydocfodder.cpython-311.pyc
    │   │       │   │   ├── pydoc_mod.cpython-311.opt-1.pyc
    │   │       │   │   ├── pydoc_mod.cpython-311.opt-2.pyc
    │   │       │   │   ├── pydoc_mod.cpython-311.pyc
    │   │       │   │   ├── pythoninfo.cpython-311.opt-1.pyc
    │   │       │   │   ├── pythoninfo.cpython-311.opt-2.pyc
    │   │       │   │   ├── pythoninfo.cpython-311.pyc
    │   │       │   │   ├── regrtest.cpython-311.opt-1.pyc
    │   │       │   │   ├── regrtest.cpython-311.opt-2.pyc
    │   │       │   │   ├── regrtest.cpython-311.pyc
    │   │       │   │   ├── relimport.cpython-311.opt-1.pyc
    │   │       │   │   ├── relimport.cpython-311.opt-2.pyc
    │   │       │   │   ├── relimport.cpython-311.pyc
    │   │       │   │   ├── reperf.cpython-311.opt-1.pyc
    │   │       │   │   ├── reperf.cpython-311.opt-2.pyc
    │   │       │   │   ├── reperf.cpython-311.pyc
    │   │       │   │   ├── re_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── re_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── re_tests.cpython-311.pyc
    │   │       │   │   ├── sample_doctest.cpython-311.opt-1.pyc
    │   │       │   │   ├── sample_doctest.cpython-311.opt-2.pyc
    │   │       │   │   ├── sample_doctest.cpython-311.pyc
    │   │       │   │   ├── sample_doctest_no_docstrings.cpython-311.opt-1.pyc
    │   │       │   │   ├── sample_doctest_no_docstrings.cpython-311.opt-2.pyc
    │   │       │   │   ├── sample_doctest_no_docstrings.cpython-311.pyc
    │   │       │   │   ├── sample_doctest_no_doctests.cpython-311.opt-1.pyc
    │   │       │   │   ├── sample_doctest_no_doctests.cpython-311.opt-2.pyc
    │   │       │   │   ├── sample_doctest_no_doctests.cpython-311.pyc
    │   │       │   │   ├── seq_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── seq_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── seq_tests.cpython-311.pyc
    │   │       │   │   ├── setup_testcppext.cpython-311.opt-1.pyc
    │   │       │   │   ├── setup_testcppext.cpython-311.opt-2.pyc
    │   │       │   │   ├── setup_testcppext.cpython-311.pyc
    │   │       │   │   ├── signalinterproctester.cpython-311.opt-1.pyc
    │   │       │   │   ├── signalinterproctester.cpython-311.opt-2.pyc
    │   │       │   │   ├── signalinterproctester.cpython-311.pyc
    │   │       │   │   ├── sortperf.cpython-311.opt-1.pyc
    │   │       │   │   ├── sortperf.cpython-311.opt-2.pyc
    │   │       │   │   ├── sortperf.cpython-311.pyc
    │   │       │   │   ├── ssl_servers.cpython-311.opt-1.pyc
    │   │       │   │   ├── ssl_servers.cpython-311.opt-2.pyc
    │   │       │   │   ├── ssl_servers.cpython-311.pyc
    │   │       │   │   ├── ssltests.cpython-311.opt-1.pyc
    │   │       │   │   ├── ssltests.cpython-311.opt-2.pyc
    │   │       │   │   ├── ssltests.cpython-311.pyc
    │   │       │   │   ├── string_tests.cpython-311.opt-1.pyc
    │   │       │   │   ├── string_tests.cpython-311.opt-2.pyc
    │   │       │   │   ├── string_tests.cpython-311.pyc
    │   │       │   │   ├── test_abc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_abc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_abc.cpython-311.pyc
    │   │       │   │   ├── test_abstract_numbers.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_abstract_numbers.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_abstract_numbers.cpython-311.pyc
    │   │       │   │   ├── test_aifc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_aifc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_aifc.cpython-311.pyc
    │   │       │   │   ├── test___all__.cpython-311.opt-1.pyc
    │   │       │   │   ├── test___all__.cpython-311.opt-2.pyc
    │   │       │   │   ├── test___all__.cpython-311.pyc
    │   │       │   │   ├── test_argparse.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_argparse.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_argparse.cpython-311.pyc
    │   │       │   │   ├── test_array.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_array.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_array.cpython-311.pyc
    │   │       │   │   ├── test_asdl_parser.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_asdl_parser.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_asdl_parser.cpython-311.pyc
    │   │       │   │   ├── test_ast.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ast.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ast.cpython-311.pyc
    │   │       │   │   ├── test_asyncgen.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_asyncgen.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_asyncgen.cpython-311.pyc
    │   │       │   │   ├── test_asynchat.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_asynchat.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_asynchat.cpython-311.pyc
    │   │       │   │   ├── test_asyncore.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_asyncore.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_asyncore.cpython-311.pyc
    │   │       │   │   ├── _test_atexit.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_atexit.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_atexit.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_atexit.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_atexit.cpython-311.pyc
    │   │       │   │   ├── test_atexit.cpython-311.pyc
    │   │       │   │   ├── test_audioop.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_audioop.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_audioop.cpython-311.pyc
    │   │       │   │   ├── test_audit.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_audit.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_audit.cpython-311.pyc
    │   │       │   │   ├── test_augassign.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_augassign.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_augassign.cpython-311.pyc
    │   │       │   │   ├── test_base64.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_base64.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_base64.cpython-311.pyc
    │   │       │   │   ├── test_baseexception.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_baseexception.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_baseexception.cpython-311.pyc
    │   │       │   │   ├── test_bdb.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bdb.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bdb.cpython-311.pyc
    │   │       │   │   ├── test_bigaddrspace.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bigaddrspace.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bigaddrspace.cpython-311.pyc
    │   │       │   │   ├── test_bigmem.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bigmem.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bigmem.cpython-311.pyc
    │   │       │   │   ├── test_binascii.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_binascii.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_binascii.cpython-311.pyc
    │   │       │   │   ├── test_binop.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_binop.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_binop.cpython-311.pyc
    │   │       │   │   ├── test_bisect.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bisect.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bisect.cpython-311.pyc
    │   │       │   │   ├── test_bool.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bool.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bool.cpython-311.pyc
    │   │       │   │   ├── test_buffer.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_buffer.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_buffer.cpython-311.pyc
    │   │       │   │   ├── test_bufio.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bufio.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bufio.cpython-311.pyc
    │   │       │   │   ├── test_builtin.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_builtin.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_builtin.cpython-311.pyc
    │   │       │   │   ├── test_bytes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bytes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bytes.cpython-311.pyc
    │   │       │   │   ├── test_bz2.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_bz2.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_bz2.cpython-311.pyc
    │   │       │   │   ├── test_calendar.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_calendar.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_calendar.cpython-311.pyc
    │   │       │   │   ├── test_call.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_call.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_call.cpython-311.pyc
    │   │       │   │   ├── test_cgi.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cgi.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cgi.cpython-311.pyc
    │   │       │   │   ├── test_cgitb.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cgitb.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cgitb.cpython-311.pyc
    │   │       │   │   ├── test_charmapcodec.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_charmapcodec.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_charmapcodec.cpython-311.pyc
    │   │       │   │   ├── test_check_c_globals.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_check_c_globals.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_check_c_globals.cpython-311.pyc
    │   │       │   │   ├── test_class.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_class.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_class.cpython-311.pyc
    │   │       │   │   ├── test_clinic.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_clinic.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_clinic.cpython-311.pyc
    │   │       │   │   ├── test_c_locale_coercion.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_c_locale_coercion.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_c_locale_coercion.cpython-311.pyc
    │   │       │   │   ├── test_cmath.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cmath.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cmath.cpython-311.pyc
    │   │       │   │   ├── test_cmd.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cmd.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cmd.cpython-311.pyc
    │   │       │   │   ├── test_cmd_line.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cmd_line.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cmd_line.cpython-311.pyc
    │   │       │   │   ├── test_cmd_line_script.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cmd_line_script.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cmd_line_script.cpython-311.pyc
    │   │       │   │   ├── test_codeccallbacks.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codeccallbacks.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codeccallbacks.cpython-311.pyc
    │   │       │   │   ├── testcodec.cpython-311.opt-1.pyc
    │   │       │   │   ├── testcodec.cpython-311.opt-2.pyc
    │   │       │   │   ├── testcodec.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_cn.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_cn.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_cn.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_hk.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_hk.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_hk.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_iso2022.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_iso2022.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_iso2022.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_jp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_jp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_jp.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_kr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_kr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_kr.cpython-311.pyc
    │   │       │   │   ├── test_codecencodings_tw.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecencodings_tw.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecencodings_tw.cpython-311.pyc
    │   │       │   │   ├── test_codecmaps_cn.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecmaps_cn.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecmaps_cn.cpython-311.pyc
    │   │       │   │   ├── test_codecmaps_hk.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecmaps_hk.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecmaps_hk.cpython-311.pyc
    │   │       │   │   ├── test_codecmaps_jp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecmaps_jp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecmaps_jp.cpython-311.pyc
    │   │       │   │   ├── test_codecmaps_kr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecmaps_kr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecmaps_kr.cpython-311.pyc
    │   │       │   │   ├── test_codecmaps_tw.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecmaps_tw.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecmaps_tw.cpython-311.pyc
    │   │       │   │   ├── test_code.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_code.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_code.cpython-311.pyc
    │   │       │   │   ├── test_codecs.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codecs.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codecs.cpython-311.pyc
    │   │       │   │   ├── test_code_module.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_code_module.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_code_module.cpython-311.pyc
    │   │       │   │   ├── test_codeop.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_codeop.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_codeop.cpython-311.pyc
    │   │       │   │   ├── test_collections.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_collections.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_collections.cpython-311.pyc
    │   │       │   │   ├── test_colorsys.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_colorsys.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_colorsys.cpython-311.pyc
    │   │       │   │   ├── test_compare.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_compare.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_compare.cpython-311.pyc
    │   │       │   │   ├── test_compileall.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_compileall.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_compileall.cpython-311.pyc
    │   │       │   │   ├── test_compile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_compile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_compile.cpython-311.pyc
    │   │       │   │   ├── test_complex.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_complex.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_complex.cpython-311.pyc
    │   │       │   │   ├── test_concurrent_futures.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_concurrent_futures.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_concurrent_futures.cpython-311.pyc
    │   │       │   │   ├── test_configparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_configparser.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_configparser.cpython-311.pyc
    │   │       │   │   ├── test_contains.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_contains.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_contains.cpython-311.pyc
    │   │       │   │   ├── test_context.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_context.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_context.cpython-311.pyc
    │   │       │   │   ├── test_contextlib_async.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_contextlib_async.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_contextlib_async.cpython-311.pyc
    │   │       │   │   ├── test_contextlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_contextlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_contextlib.cpython-311.pyc
    │   │       │   │   ├── test_copy.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_copy.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_copy.cpython-311.pyc
    │   │       │   │   ├── test_copyreg.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_copyreg.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_copyreg.cpython-311.pyc
    │   │       │   │   ├── test_coroutines.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_coroutines.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_coroutines.cpython-311.pyc
    │   │       │   │   ├── test_cppext.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cppext.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cppext.cpython-311.pyc
    │   │       │   │   ├── test_cprofile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_cprofile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_cprofile.cpython-311.pyc
    │   │       │   │   ├── test_crashers.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_crashers.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_crashers.cpython-311.pyc
    │   │       │   │   ├── test_crypt.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_crypt.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_crypt.cpython-311.pyc
    │   │       │   │   ├── test_csv.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_csv.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_csv.cpython-311.pyc
    │   │       │   │   ├── test_ctypes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ctypes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ctypes.cpython-311.pyc
    │   │       │   │   ├── test_curses.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_curses.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_curses.cpython-311.pyc
    │   │       │   │   ├── test_dataclasses.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dataclasses.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dataclasses.cpython-311.pyc
    │   │       │   │   ├── test_datetime.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_datetime.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_datetime.cpython-311.pyc
    │   │       │   │   ├── test_dbm.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dbm.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dbm.cpython-311.pyc
    │   │       │   │   ├── test_dbm_dumb.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dbm_dumb.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dbm_dumb.cpython-311.pyc
    │   │       │   │   ├── test_dbm_gnu.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dbm_gnu.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dbm_gnu.cpython-311.pyc
    │   │       │   │   ├── test_dbm_ndbm.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dbm_ndbm.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dbm_ndbm.cpython-311.pyc
    │   │       │   │   ├── test_decimal.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_decimal.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_decimal.cpython-311.pyc
    │   │       │   │   ├── test_decorators.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_decorators.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_decorators.cpython-311.pyc
    │   │       │   │   ├── test_defaultdict.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_defaultdict.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_defaultdict.cpython-311.pyc
    │   │       │   │   ├── test_deque.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_deque.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_deque.cpython-311.pyc
    │   │       │   │   ├── test_descr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_descr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_descr.cpython-311.pyc
    │   │       │   │   ├── test_descrtut.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_descrtut.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_descrtut.cpython-311.pyc
    │   │       │   │   ├── test_devpoll.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_devpoll.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_devpoll.cpython-311.pyc
    │   │       │   │   ├── test_dictcomps.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dictcomps.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dictcomps.cpython-311.pyc
    │   │       │   │   ├── test_dict.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dict.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dict.cpython-311.pyc
    │   │       │   │   ├── test_dict_version.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dict_version.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dict_version.cpython-311.pyc
    │   │       │   │   ├── test_dictviews.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dictviews.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dictviews.cpython-311.pyc
    │   │       │   │   ├── test_difflib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_difflib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_difflib.cpython-311.pyc
    │   │       │   │   ├── test_dis.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dis.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dis.cpython-311.pyc
    │   │       │   │   ├── test_distutils.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_distutils.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_distutils.cpython-311.pyc
    │   │       │   │   ├── test_doctest2.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_doctest2.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_doctest2.cpython-311.pyc
    │   │       │   │   ├── test_doctest.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_doctest.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_doctest.cpython-311.pyc
    │   │       │   │   ├── test_docxmlrpc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_docxmlrpc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_docxmlrpc.cpython-311.pyc
    │   │       │   │   ├── test_dtrace.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dtrace.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dtrace.cpython-311.pyc
    │   │       │   │   ├── test_dynamicclassattribute.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dynamicclassattribute.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dynamicclassattribute.cpython-311.pyc
    │   │       │   │   ├── test_dynamic.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_dynamic.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_dynamic.cpython-311.pyc
    │   │       │   │   ├── _test_eintr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_eintr.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_eintr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_eintr.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_eintr.cpython-311.pyc
    │   │       │   │   ├── test_eintr.cpython-311.pyc
    │   │       │   │   ├── test_embed.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_embed.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_embed.cpython-311.pyc
    │   │       │   │   ├── _test_embed_set_config.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_embed_set_config.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_embed_set_config.cpython-311.pyc
    │   │       │   │   ├── _test_embed_structseq.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_embed_structseq.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_embed_structseq.cpython-311.pyc
    │   │       │   │   ├── test_ensurepip.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ensurepip.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ensurepip.cpython-311.pyc
    │   │       │   │   ├── test_enum.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_enum.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_enum.cpython-311.pyc
    │   │       │   │   ├── test_enumerate.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_enumerate.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_enumerate.cpython-311.pyc
    │   │       │   │   ├── test_eof.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_eof.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_eof.cpython-311.pyc
    │   │       │   │   ├── test_epoll.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_epoll.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_epoll.cpython-311.pyc
    │   │       │   │   ├── test_errno.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_errno.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_errno.cpython-311.pyc
    │   │       │   │   ├── test_exception_group.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_exception_group.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_exception_group.cpython-311.pyc
    │   │       │   │   ├── test_exception_hierarchy.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_exception_hierarchy.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_exception_hierarchy.cpython-311.pyc
    │   │       │   │   ├── test_exceptions.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_exceptions.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_exceptions.cpython-311.pyc
    │   │       │   │   ├── test_exception_variations.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_exception_variations.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_exception_variations.cpython-311.pyc
    │   │       │   │   ├── test_except_star.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_except_star.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_except_star.cpython-311.pyc
    │   │       │   │   ├── test_extcall.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_extcall.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_extcall.cpython-311.pyc
    │   │       │   │   ├── test_faulthandler.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_faulthandler.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_faulthandler.cpython-311.pyc
    │   │       │   │   ├── test_fcntl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fcntl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fcntl.cpython-311.pyc
    │   │       │   │   ├── test_filecmp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_filecmp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_filecmp.cpython-311.pyc
    │   │       │   │   ├── test_file.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_file.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_file.cpython-311.pyc
    │   │       │   │   ├── test_file_eintr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_file_eintr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_file_eintr.cpython-311.pyc
    │   │       │   │   ├── test_fileinput.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fileinput.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fileinput.cpython-311.pyc
    │   │       │   │   ├── test_fileio.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fileio.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fileio.cpython-311.pyc
    │   │       │   │   ├── test_fileutils.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fileutils.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fileutils.cpython-311.pyc
    │   │       │   │   ├── test_finalization.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_finalization.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_finalization.cpython-311.pyc
    │   │       │   │   ├── test_float.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_float.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_float.cpython-311.pyc
    │   │       │   │   ├── test_flufl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_flufl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_flufl.cpython-311.pyc
    │   │       │   │   ├── test_fnmatch.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fnmatch.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fnmatch.cpython-311.pyc
    │   │       │   │   ├── test_fork1.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fork1.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fork1.cpython-311.pyc
    │   │       │   │   ├── test_format.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_format.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_format.cpython-311.pyc
    │   │       │   │   ├── test_fractions.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fractions.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fractions.cpython-311.pyc
    │   │       │   │   ├── test_frame.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_frame.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_frame.cpython-311.pyc
    │   │       │   │   ├── test_frozen.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_frozen.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_frozen.cpython-311.pyc
    │   │       │   │   ├── test_fstring.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_fstring.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_fstring.cpython-311.pyc
    │   │       │   │   ├── test_ftplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ftplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ftplib.cpython-311.pyc
    │   │       │   │   ├── test_funcattrs.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_funcattrs.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_funcattrs.cpython-311.pyc
    │   │       │   │   ├── test_functools.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_functools.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_functools.cpython-311.pyc
    │   │       │   │   ├── test_future3.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_future3.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_future3.cpython-311.pyc
    │   │       │   │   ├── test_future4.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_future4.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_future4.cpython-311.pyc
    │   │       │   │   ├── test_future5.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_future5.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_future5.cpython-311.pyc
    │   │       │   │   ├── test___future__.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_future.cpython-311.opt-1.pyc
    │   │       │   │   ├── test___future__.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_future.cpython-311.opt-2.pyc
    │   │       │   │   ├── test___future__.cpython-311.pyc
    │   │       │   │   ├── test_future.cpython-311.pyc
    │   │       │   │   ├── test_gc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_gc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_gc.cpython-311.pyc
    │   │       │   │   ├── test_gdb.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_gdb.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_gdb.cpython-311.pyc
    │   │       │   │   ├── test_generators.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_generators.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_generators.cpython-311.pyc
    │   │       │   │   ├── test_generator_stop.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_generator_stop.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_generator_stop.cpython-311.pyc
    │   │       │   │   ├── test_genericalias.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_genericalias.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_genericalias.cpython-311.pyc
    │   │       │   │   ├── test_genericclass.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_genericclass.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_genericclass.cpython-311.pyc
    │   │       │   │   ├── test_genericpath.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_genericpath.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_genericpath.cpython-311.pyc
    │   │       │   │   ├── test_genexps.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_genexps.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_genexps.cpython-311.pyc
    │   │       │   │   ├── test_getopt.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_getopt.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_getopt.cpython-311.pyc
    │   │       │   │   ├── test_getpass.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_getpass.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_getpass.cpython-311.pyc
    │   │       │   │   ├── test_getpath.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_getpath.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_getpath.cpython-311.pyc
    │   │       │   │   ├── test_gettext.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_gettext.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_gettext.cpython-311.pyc
    │   │       │   │   ├── test_global.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_global.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_global.cpython-311.pyc
    │   │       │   │   ├── test_glob.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_glob.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_glob.cpython-311.pyc
    │   │       │   │   ├── test_grammar.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_grammar.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_grammar.cpython-311.pyc
    │   │       │   │   ├── test_graphlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_graphlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_graphlib.cpython-311.pyc
    │   │       │   │   ├── test_grp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_grp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_grp.cpython-311.pyc
    │   │       │   │   ├── test_gzip.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_gzip.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_gzip.cpython-311.pyc
    │   │       │   │   ├── test_hash.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_hash.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_hash.cpython-311.pyc
    │   │       │   │   ├── test_hashlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_hashlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_hashlib.cpython-311.pyc
    │   │       │   │   ├── test_heapq.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_heapq.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_heapq.cpython-311.pyc
    │   │       │   │   ├── test_hmac.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_hmac.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_hmac.cpython-311.pyc
    │   │       │   │   ├── test_html.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_html.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_html.cpython-311.pyc
    │   │       │   │   ├── test_htmlparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_htmlparser.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_htmlparser.cpython-311.pyc
    │   │       │   │   ├── test_http_cookiejar.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_http_cookiejar.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_http_cookiejar.cpython-311.pyc
    │   │       │   │   ├── test_http_cookies.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_http_cookies.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_http_cookies.cpython-311.pyc
    │   │       │   │   ├── test_httplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_httplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_httplib.cpython-311.pyc
    │   │       │   │   ├── test_httpservers.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_httpservers.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_httpservers.cpython-311.pyc
    │   │       │   │   ├── test_idle.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_idle.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_idle.cpython-311.pyc
    │   │       │   │   ├── test_imaplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_imaplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_imaplib.cpython-311.pyc
    │   │       │   │   ├── test_imghdr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_imghdr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_imghdr.cpython-311.pyc
    │   │       │   │   ├── test_imp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_imp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_imp.cpython-311.pyc
    │   │       │   │   ├── test_index.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_index.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_index.cpython-311.pyc
    │   │       │   │   ├── test_inspect.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_inspect.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_inspect.cpython-311.pyc
    │   │       │   │   ├── test_int.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_int.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_int.cpython-311.pyc
    │   │       │   │   ├── test_interpreters.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_interpreters.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_interpreters.cpython-311.pyc
    │   │       │   │   ├── test_int_literal.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_int_literal.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_int_literal.cpython-311.pyc
    │   │       │   │   ├── test_io.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_io.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_io.cpython-311.pyc
    │   │       │   │   ├── test_ioctl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ioctl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ioctl.cpython-311.pyc
    │   │       │   │   ├── test_ipaddress.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ipaddress.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ipaddress.cpython-311.pyc
    │   │       │   │   ├── test_isinstance.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_isinstance.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_isinstance.cpython-311.pyc
    │   │       │   │   ├── test_iter.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_iter.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_iter.cpython-311.pyc
    │   │       │   │   ├── test_iterlen.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_iterlen.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_iterlen.cpython-311.pyc
    │   │       │   │   ├── test_itertools.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_itertools.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_itertools.cpython-311.pyc
    │   │       │   │   ├── test_keyword.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_keyword.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_keyword.cpython-311.pyc
    │   │       │   │   ├── test_keywordonlyarg.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_keywordonlyarg.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_keywordonlyarg.cpython-311.pyc
    │   │       │   │   ├── test_kqueue.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_kqueue.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_kqueue.cpython-311.pyc
    │   │       │   │   ├── test_largefile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_largefile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_largefile.cpython-311.pyc
    │   │       │   │   ├── test_launcher.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_launcher.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_launcher.cpython-311.pyc
    │   │       │   │   ├── test_lib2to3.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_lib2to3.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_lib2to3.cpython-311.pyc
    │   │       │   │   ├── test_linecache.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_linecache.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_linecache.cpython-311.pyc
    │   │       │   │   ├── test_listcomps.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_listcomps.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_listcomps.cpython-311.pyc
    │   │       │   │   ├── test_list.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_list.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_list.cpython-311.pyc
    │   │       │   │   ├── test_lltrace.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_lltrace.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_lltrace.cpython-311.pyc
    │   │       │   │   ├── test__locale.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_locale.cpython-311.opt-1.pyc
    │   │       │   │   ├── test__locale.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_locale.cpython-311.opt-2.pyc
    │   │       │   │   ├── test__locale.cpython-311.pyc
    │   │       │   │   ├── test_locale.cpython-311.pyc
    │   │       │   │   ├── test_logging.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_logging.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_logging.cpython-311.pyc
    │   │       │   │   ├── test_long.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_long.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_long.cpython-311.pyc
    │   │       │   │   ├── test_longexp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_longexp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_longexp.cpython-311.pyc
    │   │       │   │   ├── test_lzma.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_lzma.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_lzma.cpython-311.pyc
    │   │       │   │   ├── test_mailbox.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_mailbox.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_mailbox.cpython-311.pyc
    │   │       │   │   ├── test_mailcap.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_mailcap.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_mailcap.cpython-311.pyc
    │   │       │   │   ├── test_marshal.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_marshal.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_marshal.cpython-311.pyc
    │   │       │   │   ├── test_math.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_math.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_math.cpython-311.pyc
    │   │       │   │   ├── test_memoryio.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_memoryio.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_memoryio.cpython-311.pyc
    │   │       │   │   ├── test_memoryview.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_memoryview.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_memoryview.cpython-311.pyc
    │   │       │   │   ├── test_metaclass.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_metaclass.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_metaclass.cpython-311.pyc
    │   │       │   │   ├── test_mimetypes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_mimetypes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_mimetypes.cpython-311.pyc
    │   │       │   │   ├── test_minidom.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_minidom.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_minidom.cpython-311.pyc
    │   │       │   │   ├── test_mmap.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_mmap.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_mmap.cpython-311.pyc
    │   │       │   │   ├── test_module.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_module.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_module.cpython-311.pyc
    │   │       │   │   ├── test_modulefinder.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_modulefinder.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_modulefinder.cpython-311.pyc
    │   │       │   │   ├── test_msilib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_msilib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_msilib.cpython-311.pyc
    │   │       │   │   ├── test_multibytecodec.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_multibytecodec.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_multibytecodec.cpython-311.pyc
    │   │       │   │   ├── _test_multiprocessing.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_multiprocessing.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_multiprocessing.cpython-311.pyc
    │   │       │   │   ├── test_multiprocessing_fork.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_multiprocessing_fork.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_multiprocessing_fork.cpython-311.pyc
    │   │       │   │   ├── test_multiprocessing_forkserver.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_multiprocessing_forkserver.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_multiprocessing_forkserver.cpython-311.pyc
    │   │       │   │   ├── test_multiprocessing_main_handling.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_multiprocessing_main_handling.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_multiprocessing_main_handling.cpython-311.pyc
    │   │       │   │   ├── test_multiprocessing_spawn.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_multiprocessing_spawn.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_multiprocessing_spawn.cpython-311.pyc
    │   │       │   │   ├── test_named_expressions.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_named_expressions.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_named_expressions.cpython-311.pyc
    │   │       │   │   ├── test_netrc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_netrc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_netrc.cpython-311.pyc
    │   │       │   │   ├── test_nis.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_nis.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_nis.cpython-311.pyc
    │   │       │   │   ├── test_nntplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_nntplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_nntplib.cpython-311.pyc
    │   │       │   │   ├── test_ntpath.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ntpath.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ntpath.cpython-311.pyc
    │   │       │   │   ├── test_numeric_tower.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_numeric_tower.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_numeric_tower.cpython-311.pyc
    │   │       │   │   ├── test_opcache.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_opcache.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_opcache.cpython-311.pyc
    │   │       │   │   ├── test__opcode.cpython-311.opt-1.pyc
    │   │       │   │   ├── test__opcode.cpython-311.opt-2.pyc
    │   │       │   │   ├── test__opcode.cpython-311.pyc
    │   │       │   │   ├── test_opcodes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_opcodes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_opcodes.cpython-311.pyc
    │   │       │   │   ├── test_openpty.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_openpty.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_openpty.cpython-311.pyc
    │   │       │   │   ├── test_operator.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_operator.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_operator.cpython-311.pyc
    │   │       │   │   ├── test_optparse.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_optparse.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_optparse.cpython-311.pyc
    │   │       │   │   ├── test_ordered_dict.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ordered_dict.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ordered_dict.cpython-311.pyc
    │   │       │   │   ├── test_os.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_os.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_os.cpython-311.pyc
    │   │       │   │   ├── test_ossaudiodev.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ossaudiodev.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ossaudiodev.cpython-311.pyc
    │   │       │   │   ├── test_osx_env.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_osx_env.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_osx_env.cpython-311.pyc
    │   │       │   │   ├── test__osx_support.cpython-311.opt-1.pyc
    │   │       │   │   ├── test__osx_support.cpython-311.opt-2.pyc
    │   │       │   │   ├── test__osx_support.cpython-311.pyc
    │   │       │   │   ├── test_pathlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pathlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pathlib.cpython-311.pyc
    │   │       │   │   ├── test_patma.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_patma.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_patma.cpython-311.pyc
    │   │       │   │   ├── test_pdb.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pdb.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pdb.cpython-311.pyc
    │   │       │   │   ├── test_peepholer.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_peepholer.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_peepholer.cpython-311.pyc
    │   │       │   │   ├── test_pep646_syntax.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pep646_syntax.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pep646_syntax.cpython-311.pyc
    │   │       │   │   ├── test_picklebuffer.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_picklebuffer.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_picklebuffer.cpython-311.pyc
    │   │       │   │   ├── test_pickle.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pickle.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pickle.cpython-311.pyc
    │   │       │   │   ├── test_pickletools.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pickletools.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pickletools.cpython-311.pyc
    │   │       │   │   ├── test_pipes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pipes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pipes.cpython-311.pyc
    │   │       │   │   ├── test_pkg.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pkg.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pkg.cpython-311.pyc
    │   │       │   │   ├── test_pkgutil.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pkgutil.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pkgutil.cpython-311.pyc
    │   │       │   │   ├── test_platform.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_platform.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_platform.cpython-311.pyc
    │   │       │   │   ├── test_plistlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_plistlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_plistlib.cpython-311.pyc
    │   │       │   │   ├── test_poll.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_poll.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_poll.cpython-311.pyc
    │   │       │   │   ├── test_popen.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_popen.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_popen.cpython-311.pyc
    │   │       │   │   ├── test_poplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_poplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_poplib.cpython-311.pyc
    │   │       │   │   ├── test_positional_only_arg.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_positional_only_arg.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_positional_only_arg.cpython-311.pyc
    │   │       │   │   ├── test_posix.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_posix.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_posix.cpython-311.pyc
    │   │       │   │   ├── test_posixpath.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_posixpath.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_posixpath.cpython-311.pyc
    │   │       │   │   ├── test_pow.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pow.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pow.cpython-311.pyc
    │   │       │   │   ├── test_pprint.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pprint.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pprint.cpython-311.pyc
    │   │       │   │   ├── test_print.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_print.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_print.cpython-311.pyc
    │   │       │   │   ├── test_profile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_profile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_profile.cpython-311.pyc
    │   │       │   │   ├── test_property.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_property.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_property.cpython-311.pyc
    │   │       │   │   ├── test_pstats.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pstats.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pstats.cpython-311.pyc
    │   │       │   │   ├── test_pty.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pty.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pty.cpython-311.pyc
    │   │       │   │   ├── test_pulldom.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pulldom.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pulldom.cpython-311.pyc
    │   │       │   │   ├── test_pwd.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pwd.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pwd.cpython-311.pyc
    │   │       │   │   ├── test_pyclbr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pyclbr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pyclbr.cpython-311.pyc
    │   │       │   │   ├── test_py_compile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_py_compile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_py_compile.cpython-311.pyc
    │   │       │   │   ├── test_pydoc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pydoc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pydoc.cpython-311.pyc
    │   │       │   │   ├── test_pyexpat.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_pyexpat.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_pyexpat.cpython-311.pyc
    │   │       │   │   ├── test_queue.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_queue.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_queue.cpython-311.pyc
    │   │       │   │   ├── test_quopri.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_quopri.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_quopri.cpython-311.pyc
    │   │       │   │   ├── test_raise.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_raise.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_raise.cpython-311.pyc
    │   │       │   │   ├── test_random.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_random.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_random.cpython-311.pyc
    │   │       │   │   ├── test_range.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_range.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_range.cpython-311.pyc
    │   │       │   │   ├── test_readline.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_readline.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_readline.cpython-311.pyc
    │   │       │   │   ├── test_re.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_re.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_re.cpython-311.pyc
    │   │       │   │   ├── test_regrtest.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_regrtest.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_regrtest.cpython-311.pyc
    │   │       │   │   ├── test_repl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_repl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_repl.cpython-311.pyc
    │   │       │   │   ├── test_reprlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_reprlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_reprlib.cpython-311.pyc
    │   │       │   │   ├── test_resource.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_resource.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_resource.cpython-311.pyc
    │   │       │   │   ├── test_richcmp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_richcmp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_richcmp.cpython-311.pyc
    │   │       │   │   ├── test_rlcompleter.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_rlcompleter.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_rlcompleter.cpython-311.pyc
    │   │       │   │   ├── test_robotparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_robotparser.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_robotparser.cpython-311.pyc
    │   │       │   │   ├── test_runpy.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_runpy.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_runpy.cpython-311.pyc
    │   │       │   │   ├── test_sax.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sax.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sax.cpython-311.pyc
    │   │       │   │   ├── test_sched.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sched.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sched.cpython-311.pyc
    │   │       │   │   ├── test_scope.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_scope.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_scope.cpython-311.pyc
    │   │       │   │   ├── test_script_helper.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_script_helper.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_script_helper.cpython-311.pyc
    │   │       │   │   ├── test_secrets.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_secrets.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_secrets.cpython-311.pyc
    │   │       │   │   ├── test_select.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_select.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_select.cpython-311.pyc
    │   │       │   │   ├── test_selectors.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_selectors.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_selectors.cpython-311.pyc
    │   │       │   │   ├── test_setcomps.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_setcomps.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_setcomps.cpython-311.pyc
    │   │       │   │   ├── test_set.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_set.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_set.cpython-311.pyc
    │   │       │   │   ├── test_shelve.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_shelve.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_shelve.cpython-311.pyc
    │   │       │   │   ├── test_shlex.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_shlex.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_shlex.cpython-311.pyc
    │   │       │   │   ├── test_shutil.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_shutil.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_shutil.cpython-311.pyc
    │   │       │   │   ├── test_signal.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_signal.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_signal.cpython-311.pyc
    │   │       │   │   ├── test_site.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_site.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_site.cpython-311.pyc
    │   │       │   │   ├── test_slice.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_slice.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_slice.cpython-311.pyc
    │   │       │   │   ├── test_smtpd.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_smtpd.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_smtpd.cpython-311.pyc
    │   │       │   │   ├── test_smtplib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_smtplib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_smtplib.cpython-311.pyc
    │   │       │   │   ├── test_smtpnet.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_smtpnet.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_smtpnet.cpython-311.pyc
    │   │       │   │   ├── test_sndhdr.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sndhdr.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sndhdr.cpython-311.pyc
    │   │       │   │   ├── test_socket.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_socket.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_socket.cpython-311.pyc
    │   │       │   │   ├── test_socketserver.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_socketserver.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_socketserver.cpython-311.pyc
    │   │       │   │   ├── test_sort.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sort.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sort.cpython-311.pyc
    │   │       │   │   ├── test_source_encoding.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_source_encoding.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_source_encoding.cpython-311.pyc
    │   │       │   │   ├── test_spwd.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_spwd.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_spwd.cpython-311.pyc
    │   │       │   │   ├── test_ssl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ssl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ssl.cpython-311.pyc
    │   │       │   │   ├── test_stable_abi_ctypes.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_stable_abi_ctypes.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_stable_abi_ctypes.cpython-311.pyc
    │   │       │   │   ├── test_startfile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_startfile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_startfile.cpython-311.pyc
    │   │       │   │   ├── test_stat.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_stat.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_stat.cpython-311.pyc
    │   │       │   │   ├── test_statistics.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_statistics.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_statistics.cpython-311.pyc
    │   │       │   │   ├── test_strftime.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_strftime.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_strftime.cpython-311.pyc
    │   │       │   │   ├── test_string.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_string.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_string.cpython-311.pyc
    │   │       │   │   ├── test_string_literals.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_string_literals.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_string_literals.cpython-311.pyc
    │   │       │   │   ├── test_stringprep.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_stringprep.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_stringprep.cpython-311.pyc
    │   │       │   │   ├── test_strptime.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_strptime.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_strptime.cpython-311.pyc
    │   │       │   │   ├── test_strtod.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_strtod.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_strtod.cpython-311.pyc
    │   │       │   │   ├── test_struct.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_struct.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_struct.cpython-311.pyc
    │   │       │   │   ├── test_structseq.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_structseq.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_structseq.cpython-311.pyc
    │   │       │   │   ├── test_subclassinit.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_subclassinit.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_subclassinit.cpython-311.pyc
    │   │       │   │   ├── test_subprocess.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_subprocess.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_subprocess.cpython-311.pyc
    │   │       │   │   ├── test_sunau.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sunau.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sunau.cpython-311.pyc
    │   │       │   │   ├── test_sundry.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sundry.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sundry.cpython-311.pyc
    │   │       │   │   ├── test_super.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_super.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_super.cpython-311.pyc
    │   │       │   │   ├── test_support.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_support.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_support.cpython-311.pyc
    │   │       │   │   ├── test_symtable.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_symtable.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_symtable.cpython-311.pyc
    │   │       │   │   ├── test_syntax.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_syntax.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_syntax.cpython-311.pyc
    │   │       │   │   ├── test_sysconfig.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sysconfig.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sysconfig.cpython-311.pyc
    │   │       │   │   ├── test_sys.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sys.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sys.cpython-311.pyc
    │   │       │   │   ├── test_syslog.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_syslog.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_syslog.cpython-311.pyc
    │   │       │   │   ├── test_sys_setprofile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sys_setprofile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sys_setprofile.cpython-311.pyc
    │   │       │   │   ├── test_sys_settrace.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_sys_settrace.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_sys_settrace.cpython-311.pyc
    │   │       │   │   ├── test_tabnanny.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tabnanny.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tabnanny.cpython-311.pyc
    │   │       │   │   ├── test_tarfile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tarfile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tarfile.cpython-311.pyc
    │   │       │   │   ├── test_tcl.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tcl.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tcl.cpython-311.pyc
    │   │       │   │   ├── test_telnetlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_telnetlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_telnetlib.cpython-311.pyc
    │   │       │   │   ├── test_tempfile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tempfile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tempfile.cpython-311.pyc
    │   │       │   │   ├── test_textwrap.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_textwrap.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_textwrap.cpython-311.pyc
    │   │       │   │   ├── test_thread.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_thread.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_thread.cpython-311.pyc
    │   │       │   │   ├── test_threadedtempfile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_threadedtempfile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_threadedtempfile.cpython-311.pyc
    │   │       │   │   ├── test_threading.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_threading.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_threading.cpython-311.pyc
    │   │       │   │   ├── test_threading_local.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_threading_local.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_threading_local.cpython-311.pyc
    │   │       │   │   ├── test_threadsignals.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_threadsignals.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_threadsignals.cpython-311.pyc
    │   │       │   │   ├── test_time.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_time.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_time.cpython-311.pyc
    │   │       │   │   ├── test_timeit.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_timeit.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_timeit.cpython-311.pyc
    │   │       │   │   ├── test_timeout.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_timeout.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_timeout.cpython-311.pyc
    │   │       │   │   ├── test_tix.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tix.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tix.cpython-311.pyc
    │   │       │   │   ├── test_tk.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tk.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tk.cpython-311.pyc
    │   │       │   │   ├── test_tokenize.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tokenize.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tokenize.cpython-311.pyc
    │   │       │   │   ├── test_traceback.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_traceback.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_traceback.cpython-311.pyc
    │   │       │   │   ├── test_trace.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_trace.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_trace.cpython-311.pyc
    │   │       │   │   ├── test_tracemalloc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tracemalloc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tracemalloc.cpython-311.pyc
    │   │       │   │   ├── test_ttk_guionly.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ttk_guionly.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ttk_guionly.cpython-311.pyc
    │   │       │   │   ├── test_ttk_textonly.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ttk_textonly.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ttk_textonly.cpython-311.pyc
    │   │       │   │   ├── test_tuple.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_tuple.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_tuple.cpython-311.pyc
    │   │       │   │   ├── test_turtle.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_turtle.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_turtle.cpython-311.pyc
    │   │       │   │   ├── test_type_annotations.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_type_annotations.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_type_annotations.cpython-311.pyc
    │   │       │   │   ├── test_type_cache.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_type_cache.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_type_cache.cpython-311.pyc
    │   │       │   │   ├── test_typechecks.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_typechecks.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_typechecks.cpython-311.pyc
    │   │       │   │   ├── test_type_comments.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_type_comments.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_type_comments.cpython-311.pyc
    │   │       │   │   ├── test_types.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_types.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_types.cpython-311.pyc
    │   │       │   │   ├── test_typing.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_typing.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_typing.cpython-311.pyc
    │   │       │   │   ├── test_ucn.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_ucn.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_ucn.cpython-311.pyc
    │   │       │   │   ├── test_unary.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unary.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unary.cpython-311.pyc
    │   │       │   │   ├── test_unicode.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unicode.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unicode.cpython-311.pyc
    │   │       │   │   ├── test_unicodedata.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unicodedata.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unicodedata.cpython-311.pyc
    │   │       │   │   ├── test_unicode_file.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unicode_file.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unicode_file.cpython-311.pyc
    │   │       │   │   ├── test_unicode_file_functions.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unicode_file_functions.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unicode_file_functions.cpython-311.pyc
    │   │       │   │   ├── test_unicode_identifiers.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unicode_identifiers.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unicode_identifiers.cpython-311.pyc
    │   │       │   │   ├── test_unittest.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unittest.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unittest.cpython-311.pyc
    │   │       │   │   ├── test_univnewlines.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_univnewlines.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_univnewlines.cpython-311.pyc
    │   │       │   │   ├── test_unpack.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unpack.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unpack.cpython-311.pyc
    │   │       │   │   ├── test_unpack_ex.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unpack_ex.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unpack_ex.cpython-311.pyc
    │   │       │   │   ├── test_unparse.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_unparse.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_unparse.cpython-311.pyc
    │   │       │   │   ├── test_urllib2.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllib2.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllib2.cpython-311.pyc
    │   │       │   │   ├── test_urllib2_localnet.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllib2_localnet.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllib2_localnet.cpython-311.pyc
    │   │       │   │   ├── test_urllib2net.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllib2net.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllib2net.cpython-311.pyc
    │   │       │   │   ├── test_urllib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllib.cpython-311.pyc
    │   │       │   │   ├── test_urllibnet.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllibnet.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllibnet.cpython-311.pyc
    │   │       │   │   ├── test_urllib_response.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urllib_response.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urllib_response.cpython-311.pyc
    │   │       │   │   ├── test_urlparse.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_urlparse.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_urlparse.cpython-311.pyc
    │   │       │   │   ├── test_userdict.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_userdict.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_userdict.cpython-311.pyc
    │   │       │   │   ├── test_userlist.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_userlist.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_userlist.cpython-311.pyc
    │   │       │   │   ├── test_userstring.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_userstring.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_userstring.cpython-311.pyc
    │   │       │   │   ├── test_utf8_mode.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_utf8_mode.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_utf8_mode.cpython-311.pyc
    │   │       │   │   ├── test_utf8source.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_utf8source.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_utf8source.cpython-311.pyc
    │   │       │   │   ├── test_uu.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_uu.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_uu.cpython-311.pyc
    │   │       │   │   ├── test_uuid.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_uuid.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_uuid.cpython-311.pyc
    │   │       │   │   ├── test_venv.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_venv.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_venv.cpython-311.pyc
    │   │       │   │   ├── _test_venv_multiprocessing.cpython-311.opt-1.pyc
    │   │       │   │   ├── _test_venv_multiprocessing.cpython-311.opt-2.pyc
    │   │       │   │   ├── _test_venv_multiprocessing.cpython-311.pyc
    │   │       │   │   ├── test_wait3.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_wait3.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_wait3.cpython-311.pyc
    │   │       │   │   ├── test_wait4.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_wait4.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_wait4.cpython-311.pyc
    │   │       │   │   ├── test_wave.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_wave.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_wave.cpython-311.pyc
    │   │       │   │   ├── test_weakref.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_weakref.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_weakref.cpython-311.pyc
    │   │       │   │   ├── test_weakset.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_weakset.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_weakset.cpython-311.pyc
    │   │       │   │   ├── test_webbrowser.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_webbrowser.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_webbrowser.cpython-311.pyc
    │   │       │   │   ├── test_winconsoleio.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_winconsoleio.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_winconsoleio.cpython-311.pyc
    │   │       │   │   ├── test_winreg.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_winreg.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_winreg.cpython-311.pyc
    │   │       │   │   ├── test_winsound.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_winsound.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_winsound.cpython-311.pyc
    │   │       │   │   ├── test_with.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_with.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_with.cpython-311.pyc
    │   │       │   │   ├── test_wsgiref.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_wsgiref.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_wsgiref.cpython-311.pyc
    │   │       │   │   ├── test_xdrlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xdrlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xdrlib.cpython-311.pyc
    │   │       │   │   ├── test_xml_dom_minicompat.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xml_dom_minicompat.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xml_dom_minicompat.cpython-311.pyc
    │   │       │   │   ├── test_xml_etree_c.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xml_etree_c.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xml_etree_c.cpython-311.pyc
    │   │       │   │   ├── test_xml_etree.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xml_etree.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xml_etree.cpython-311.pyc
    │   │       │   │   ├── test_xmlrpc.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xmlrpc.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xmlrpc.cpython-311.pyc
    │   │       │   │   ├── test_xmlrpc_net.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xmlrpc_net.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xmlrpc_net.cpython-311.pyc
    │   │       │   │   ├── test_xxlimited.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xxlimited.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xxlimited.cpython-311.pyc
    │   │       │   │   ├── test__xxsubinterpreters.cpython-311.opt-1.pyc
    │   │       │   │   ├── test__xxsubinterpreters.cpython-311.opt-2.pyc
    │   │       │   │   ├── test__xxsubinterpreters.cpython-311.pyc
    │   │       │   │   ├── test_xxtestfuzz.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_xxtestfuzz.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_xxtestfuzz.cpython-311.pyc
    │   │       │   │   ├── test_yield_from.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_yield_from.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_yield_from.cpython-311.pyc
    │   │       │   │   ├── test_zipapp.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zipapp.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zipapp.cpython-311.pyc
    │   │       │   │   ├── test_zipfile64.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zipfile64.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zipfile64.cpython-311.pyc
    │   │       │   │   ├── test_zipfile.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zipfile.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zipfile.cpython-311.pyc
    │   │       │   │   ├── test_zipimport.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zipimport.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zipimport.cpython-311.pyc
    │   │       │   │   ├── test_zipimport_support.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zipimport_support.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zipimport_support.cpython-311.pyc
    │   │       │   │   ├── test_zlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── test_zlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── test_zlib.cpython-311.pyc
    │   │       │   │   ├── tf_inherit_check.cpython-311.opt-1.pyc
    │   │       │   │   ├── tf_inherit_check.cpython-311.opt-2.pyc
    │   │       │   │   ├── tf_inherit_check.cpython-311.pyc
    │   │       │   │   ├── time_hashlib.cpython-311.opt-1.pyc
    │   │       │   │   ├── time_hashlib.cpython-311.opt-2.pyc
    │   │       │   │   ├── time_hashlib.cpython-311.pyc
    │   │       │   │   ├── _typed_dict_helper.cpython-311.opt-1.pyc
    │   │       │   │   ├── _typed_dict_helper.cpython-311.opt-2.pyc
    │   │       │   │   ├── _typed_dict_helper.cpython-311.pyc
    │   │       │   │   ├── win_console_handler.cpython-311.opt-1.pyc
    │   │       │   │   ├── win_console_handler.cpython-311.opt-2.pyc
    │   │       │   │   ├── win_console_handler.cpython-311.pyc
    │   │       │   │   ├── xmltests.cpython-311.opt-1.pyc
    │   │       │   │   ├── xmltests.cpython-311.opt-2.pyc
    │   │       │   │   └── xmltests.cpython-311.pyc
    │   │       │   ├── pycakey.pem
    │   │       │   ├── pyclbr_input.py
    │   │       │   ├── pydocfodder.py
    │   │       │   ├── pydoc_mod.py
    │   │       │   ├── pythoninfo.py
    │   │       │   ├── randv2_32.pck
    │   │       │   ├── randv2_64.pck
    │   │       │   ├── randv3.pck
    │   │       │   ├── recursion.tar
    │   │       │   ├── regrtest.py
    │   │       │   ├── relimport.py
    │   │       │   ├── reperf.py
    │   │       │   ├── re_tests.py
    │   │       │   ├── revocation.crl
    │   │       │   ├── sample_doctest_no_docstrings.py
    │   │       │   ├── sample_doctest_no_doctests.py
    │   │       │   ├── sample_doctest.py
    │   │       │   ├── secp384r1.pem
    │   │       │   ├── selfsigned_pythontestdotnet.pem
    │   │       │   ├── seq_tests.py
    │   │       │   ├── setup_testcppext.py
    │   │       │   ├── sgml_input.html
    │   │       │   ├── signalinterproctester.py
    │   │       │   ├── Sine-1000Hz-300ms.aif
    │   │       │   ├── sndhdrdata
    │   │       │   │   ├── README
    │   │       │   │   ├── sndhdr.8svx
    │   │       │   │   ├── sndhdr.aifc
    │   │       │   │   ├── sndhdr.aiff
    │   │       │   │   ├── sndhdr.au
    │   │       │   │   ├── sndhdr.hcom
    │   │       │   │   ├── sndhdr.sndt
    │   │       │   │   ├── sndhdr.voc
    │   │       │   │   └── sndhdr.wav
    │   │       │   ├── sortperf.py
    │   │       │   ├── ssl_cert.pem
    │   │       │   ├── ssl_key.passwd.pem
    │   │       │   ├── ssl_key.pem
    │   │       │   ├── ssl_servers.py
    │   │       │   ├── ssltests.py
    │   │       │   ├── string_tests.py
    │   │       │   ├── subprocessdata
    │   │       │   │   ├── fd_status.py
    │   │       │   │   ├── input_reader.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── fd_status.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── fd_status.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── fd_status.cpython-311.pyc
    │   │       │   │   │   ├── input_reader.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── input_reader.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── input_reader.cpython-311.pyc
    │   │       │   │   │   ├── qcat.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── qcat.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── qcat.cpython-311.pyc
    │   │       │   │   │   ├── qgrep.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── qgrep.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── qgrep.cpython-311.pyc
    │   │       │   │   │   ├── sigchild_ignore.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── sigchild_ignore.cpython-311.opt-2.pyc
    │   │       │   │   │   └── sigchild_ignore.cpython-311.pyc
    │   │       │   │   ├── qcat.py
    │   │       │   │   ├── qgrep.py
    │   │       │   │   └── sigchild_ignore.py
    │   │       │   ├── support
    │   │       │   │   ├── bytecode_helper.py
    │   │       │   │   ├── hashlib_helper.py
    │   │       │   │   ├── import_helper.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── interpreters.py
    │   │       │   │   ├── logging_helper.py
    │   │       │   │   ├── os_helper.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── bytecode_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── bytecode_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── bytecode_helper.cpython-311.pyc
    │   │       │   │   │   ├── hashlib_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── hashlib_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── hashlib_helper.cpython-311.pyc
    │   │       │   │   │   ├── import_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── import_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── import_helper.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── interpreters.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── interpreters.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── interpreters.cpython-311.pyc
    │   │       │   │   │   ├── logging_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── logging_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── logging_helper.cpython-311.pyc
    │   │       │   │   │   ├── os_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── os_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── os_helper.cpython-311.pyc
    │   │       │   │   │   ├── script_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── script_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── script_helper.cpython-311.pyc
    │   │       │   │   │   ├── socket_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── socket_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── socket_helper.cpython-311.pyc
    │   │       │   │   │   ├── testresult.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── testresult.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── testresult.cpython-311.pyc
    │   │       │   │   │   ├── threading_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── threading_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── threading_helper.cpython-311.pyc
    │   │       │   │   │   ├── warnings_helper.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── warnings_helper.cpython-311.opt-2.pyc
    │   │       │   │   │   └── warnings_helper.cpython-311.pyc
    │   │       │   │   ├── script_helper.py
    │   │       │   │   ├── socket_helper.py
    │   │       │   │   ├── testresult.py
    │   │       │   │   ├── threading_helper.py
    │   │       │   │   └── warnings_helper.py
    │   │       │   ├── talos-2019-0758.pem
    │   │       │   ├── test_abc.py
    │   │       │   ├── test_abstract_numbers.py
    │   │       │   ├── test_aifc.py
    │   │       │   ├── test___all__.py
    │   │       │   ├── test_argparse.py
    │   │       │   ├── test_array.py
    │   │       │   ├── test_asdl_parser.py
    │   │       │   ├── test_ast.py
    │   │       │   ├── test_asyncgen.py
    │   │       │   ├── test_asynchat.py
    │   │       │   ├── test_asyncio
    │   │       │   │   ├── echo2.py
    │   │       │   │   ├── echo3.py
    │   │       │   │   ├── echo.py
    │   │       │   │   ├── functional.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── echo2.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── echo2.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── echo2.cpython-311.pyc
    │   │       │   │   │   ├── echo3.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── echo3.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── echo3.cpython-311.pyc
    │   │       │   │   │   ├── echo.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── echo.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── echo.cpython-311.pyc
    │   │       │   │   │   ├── functional.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── functional.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── functional.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_base_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_base_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_base_events.cpython-311.pyc
    │   │       │   │   │   ├── test_buffered_proto.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_buffered_proto.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_buffered_proto.cpython-311.pyc
    │   │       │   │   │   ├── test_context.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_context.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_context.cpython-311.pyc
    │   │       │   │   │   ├── test_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_events.cpython-311.pyc
    │   │       │   │   │   ├── test_futures2.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_futures2.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_futures2.cpython-311.pyc
    │   │       │   │   │   ├── test_futures.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_futures.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_futures.cpython-311.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.pyc
    │   │       │   │   │   ├── test_pep492.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pep492.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pep492.cpython-311.pyc
    │   │       │   │   │   ├── test_proactor_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_proactor_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_proactor_events.cpython-311.pyc
    │   │       │   │   │   ├── test_protocols.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_protocols.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_protocols.cpython-311.pyc
    │   │       │   │   │   ├── test_queues.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_queues.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_queues.cpython-311.pyc
    │   │       │   │   │   ├── test_runners.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_runners.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_runners.cpython-311.pyc
    │   │       │   │   │   ├── test_selector_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_selector_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_selector_events.cpython-311.pyc
    │   │       │   │   │   ├── test_sendfile.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sendfile.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sendfile.cpython-311.pyc
    │   │       │   │   │   ├── test_server.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_server.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_server.cpython-311.pyc
    │   │       │   │   │   ├── test_sock_lowlevel.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sock_lowlevel.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sock_lowlevel.cpython-311.pyc
    │   │       │   │   │   ├── test_ssl.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_ssl.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_ssl.cpython-311.pyc
    │   │       │   │   │   ├── test_sslproto.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sslproto.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_sslproto.cpython-311.pyc
    │   │       │   │   │   ├── test_streams.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_streams.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_streams.cpython-311.pyc
    │   │       │   │   │   ├── test_subprocess.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_subprocess.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_subprocess.cpython-311.pyc
    │   │       │   │   │   ├── test_taskgroups.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_taskgroups.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_taskgroups.cpython-311.pyc
    │   │       │   │   │   ├── test_tasks.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_tasks.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_tasks.cpython-311.pyc
    │   │       │   │   │   ├── test_threads.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_threads.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_threads.cpython-311.pyc
    │   │       │   │   │   ├── test_timeouts.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_timeouts.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_timeouts.cpython-311.pyc
    │   │       │   │   │   ├── test_transports.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_transports.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_transports.cpython-311.pyc
    │   │       │   │   │   ├── test_unix_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unix_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_unix_events.cpython-311.pyc
    │   │       │   │   │   ├── test_waitfor.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_waitfor.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_waitfor.cpython-311.pyc
    │   │       │   │   │   ├── test_windows_events.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_windows_events.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_windows_events.cpython-311.pyc
    │   │       │   │   │   ├── test_windows_utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_windows_utils.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_windows_utils.cpython-311.pyc
    │   │       │   │   │   ├── utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── utils.cpython-311.opt-2.pyc
    │   │       │   │   │   └── utils.cpython-311.pyc
    │   │       │   │   ├── test_base_events.py
    │   │       │   │   ├── test_buffered_proto.py
    │   │       │   │   ├── test_context.py
    │   │       │   │   ├── test_events.py
    │   │       │   │   ├── test_futures2.py
    │   │       │   │   ├── test_futures.py
    │   │       │   │   ├── test_locks.py
    │   │       │   │   ├── test_pep492.py
    │   │       │   │   ├── test_proactor_events.py
    │   │       │   │   ├── test_protocols.py
    │   │       │   │   ├── test_queues.py
    │   │       │   │   ├── test_runners.py
    │   │       │   │   ├── test_selector_events.py
    │   │       │   │   ├── test_sendfile.py
    │   │       │   │   ├── test_server.py
    │   │       │   │   ├── test_sock_lowlevel.py
    │   │       │   │   ├── test_sslproto.py
    │   │       │   │   ├── test_ssl.py
    │   │       │   │   ├── test_streams.py
    │   │       │   │   ├── test_subprocess.py
    │   │       │   │   ├── test_taskgroups.py
    │   │       │   │   ├── test_tasks.py
    │   │       │   │   ├── test_threads.py
    │   │       │   │   ├── test_timeouts.py
    │   │       │   │   ├── test_transports.py
    │   │       │   │   ├── test_unix_events.py
    │   │       │   │   ├── test_waitfor.py
    │   │       │   │   ├── test_windows_events.py
    │   │       │   │   ├── test_windows_utils.py
    │   │       │   │   └── utils.py
    │   │       │   ├── test_asyncore.py
    │   │       │   ├── _test_atexit.py
    │   │       │   ├── test_atexit.py
    │   │       │   ├── test_audioop.py
    │   │       │   ├── test_audit.py
    │   │       │   ├── test_augassign.py
    │   │       │   ├── test_base64.py
    │   │       │   ├── test_baseexception.py
    │   │       │   ├── test_bdb.py
    │   │       │   ├── test_bigaddrspace.py
    │   │       │   ├── test_bigmem.py
    │   │       │   ├── test_binascii.py
    │   │       │   ├── test_binop.py
    │   │       │   ├── test_bisect.py
    │   │       │   ├── test_bool.py
    │   │       │   ├── test_buffer.py
    │   │       │   ├── test_bufio.py
    │   │       │   ├── test_builtin.py
    │   │       │   ├── test_bytes.py
    │   │       │   ├── test_bz2.py
    │   │       │   ├── test_calendar.py
    │   │       │   ├── test_call.py
    │   │       │   ├── test_capi
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_eval_code_ex.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_eval_code_ex.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_eval_code_ex.cpython-311.pyc
    │   │       │   │   │   ├── test_getargs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_getargs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_getargs.cpython-311.pyc
    │   │       │   │   │   ├── test_misc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_misc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_misc.cpython-311.pyc
    │   │       │   │   │   ├── test_structmembers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_structmembers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_structmembers.cpython-311.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_unicode.cpython-311.pyc
    │   │       │   │   ├── test_eval_code_ex.py
    │   │       │   │   ├── test_getargs.py
    │   │       │   │   ├── test_misc.py
    │   │       │   │   ├── test_structmembers.py
    │   │       │   │   └── test_unicode.py
    │   │       │   ├── test_cgi.py
    │   │       │   ├── test_cgitb.py
    │   │       │   ├── test_charmapcodec.py
    │   │       │   ├── test_check_c_globals.py
    │   │       │   ├── test_class.py
    │   │       │   ├── test_clinic.py
    │   │       │   ├── test_c_locale_coercion.py
    │   │       │   ├── test_cmath.py
    │   │       │   ├── test_cmd_line.py
    │   │       │   ├── test_cmd_line_script.py
    │   │       │   ├── test_cmd.py
    │   │       │   ├── test_codeccallbacks.py
    │   │       │   ├── test_codecencodings_cn.py
    │   │       │   ├── test_codecencodings_hk.py
    │   │       │   ├── test_codecencodings_iso2022.py
    │   │       │   ├── test_codecencodings_jp.py
    │   │       │   ├── test_codecencodings_kr.py
    │   │       │   ├── test_codecencodings_tw.py
    │   │       │   ├── test_codecmaps_cn.py
    │   │       │   ├── test_codecmaps_hk.py
    │   │       │   ├── test_codecmaps_jp.py
    │   │       │   ├── test_codecmaps_kr.py
    │   │       │   ├── test_codecmaps_tw.py
    │   │       │   ├── testcodec.py
    │   │       │   ├── test_codecs.py
    │   │       │   ├── test_code_module.py
    │   │       │   ├── test_codeop.py
    │   │       │   ├── test_code.py
    │   │       │   ├── test_collections.py
    │   │       │   ├── test_colorsys.py
    │   │       │   ├── test_compare.py
    │   │       │   ├── test_compileall.py
    │   │       │   ├── test_compile.py
    │   │       │   ├── test_complex.py
    │   │       │   ├── test_concurrent_futures.py
    │   │       │   ├── test_configparser.py
    │   │       │   ├── test_contains.py
    │   │       │   ├── test_contextlib_async.py
    │   │       │   ├── test_contextlib.py
    │   │       │   ├── test_context.py
    │   │       │   ├── test_copy.py
    │   │       │   ├── test_copyreg.py
    │   │       │   ├── test_coroutines.py
    │   │       │   ├── _testcppext.cpp
    │   │       │   ├── test_cppext.py
    │   │       │   ├── test_cprofile.py
    │   │       │   ├── test_crashers.py
    │   │       │   ├── test_crypt.py
    │   │       │   ├── test_csv.py
    │   │       │   ├── test_ctypes.py
    │   │       │   ├── test_curses.py
    │   │       │   ├── test_dataclasses.py
    │   │       │   ├── test_datetime.py
    │   │       │   ├── test_dbm_dumb.py
    │   │       │   ├── test_dbm_gnu.py
    │   │       │   ├── test_dbm_ndbm.py
    │   │       │   ├── test_dbm.py
    │   │       │   ├── test_decimal.py
    │   │       │   ├── test_decorators.py
    │   │       │   ├── test_defaultdict.py
    │   │       │   ├── test_deque.py
    │   │       │   ├── test_descr.py
    │   │       │   ├── test_descrtut.py
    │   │       │   ├── test_devpoll.py
    │   │       │   ├── test_dictcomps.py
    │   │       │   ├── test_dict.py
    │   │       │   ├── test_dict_version.py
    │   │       │   ├── test_dictviews.py
    │   │       │   ├── test_difflib_expect.html
    │   │       │   ├── test_difflib.py
    │   │       │   ├── test_dis.py
    │   │       │   ├── test_distutils.py
    │   │       │   ├── test_doctest2.py
    │   │       │   ├── test_doctest2.txt
    │   │       │   ├── test_doctest3.txt
    │   │       │   ├── test_doctest4.txt
    │   │       │   ├── test_doctest.py
    │   │       │   ├── test_doctest.txt
    │   │       │   ├── test_docxmlrpc.py
    │   │       │   ├── test_dtrace.py
    │   │       │   ├── test_dynamicclassattribute.py
    │   │       │   ├── test_dynamic.py
    │   │       │   ├── _test_eintr.py
    │   │       │   ├── test_eintr.py
    │   │       │   ├── test_email
    │   │       │   │   ├── data
    │   │       │   │   │   ├── msg_01.txt
    │   │       │   │   │   ├── msg_02.txt
    │   │       │   │   │   ├── msg_03.txt
    │   │       │   │   │   ├── msg_04.txt
    │   │       │   │   │   ├── msg_05.txt
    │   │       │   │   │   ├── msg_06.txt
    │   │       │   │   │   ├── msg_07.txt
    │   │       │   │   │   ├── msg_08.txt
    │   │       │   │   │   ├── msg_09.txt
    │   │       │   │   │   ├── msg_10.txt
    │   │       │   │   │   ├── msg_11.txt
    │   │       │   │   │   ├── msg_12a.txt
    │   │       │   │   │   ├── msg_12.txt
    │   │       │   │   │   ├── msg_13.txt
    │   │       │   │   │   ├── msg_14.txt
    │   │       │   │   │   ├── msg_15.txt
    │   │       │   │   │   ├── msg_16.txt
    │   │       │   │   │   ├── msg_17.txt
    │   │       │   │   │   ├── msg_18.txt
    │   │       │   │   │   ├── msg_19.txt
    │   │       │   │   │   ├── msg_20.txt
    │   │       │   │   │   ├── msg_21.txt
    │   │       │   │   │   ├── msg_22.txt
    │   │       │   │   │   ├── msg_23.txt
    │   │       │   │   │   ├── msg_24.txt
    │   │       │   │   │   ├── msg_25.txt
    │   │       │   │   │   ├── msg_26.txt
    │   │       │   │   │   ├── msg_27.txt
    │   │       │   │   │   ├── msg_28.txt
    │   │       │   │   │   ├── msg_29.txt
    │   │       │   │   │   ├── msg_30.txt
    │   │       │   │   │   ├── msg_31.txt
    │   │       │   │   │   ├── msg_32.txt
    │   │       │   │   │   ├── msg_33.txt
    │   │       │   │   │   ├── msg_34.txt
    │   │       │   │   │   ├── msg_35.txt
    │   │       │   │   │   ├── msg_36.txt
    │   │       │   │   │   ├── msg_37.txt
    │   │       │   │   │   ├── msg_38.txt
    │   │       │   │   │   ├── msg_39.txt
    │   │       │   │   │   ├── msg_40.txt
    │   │       │   │   │   ├── msg_41.txt
    │   │       │   │   │   ├── msg_42.txt
    │   │       │   │   │   ├── msg_43.txt
    │   │       │   │   │   ├── msg_44.txt
    │   │       │   │   │   ├── msg_45.txt
    │   │       │   │   │   ├── msg_46.txt
    │   │       │   │   │   ├── python.bmp
    │   │       │   │   │   ├── python.exr
    │   │       │   │   │   ├── python.gif
    │   │       │   │   │   ├── python.jpg
    │   │       │   │   │   ├── python.pbm
    │   │       │   │   │   ├── python.pgm
    │   │       │   │   │   ├── python.png
    │   │       │   │   │   ├── python.ppm
    │   │       │   │   │   ├── python.ras
    │   │       │   │   │   ├── python.sgi
    │   │       │   │   │   ├── python.tiff
    │   │       │   │   │   ├── python.webp
    │   │       │   │   │   ├── python.xbm
    │   │       │   │   │   ├── sndhdr.aifc
    │   │       │   │   │   ├── sndhdr.aiff
    │   │       │   │   │   ├── sndhdr.au
    │   │       │   │   │   └── sndhdr.wav
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_asian_codecs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_asian_codecs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_asian_codecs.cpython-311.pyc
    │   │       │   │   │   ├── test_contentmanager.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_contentmanager.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_contentmanager.cpython-311.pyc
    │   │       │   │   │   ├── test_defect_handling.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_defect_handling.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_defect_handling.cpython-311.pyc
    │   │       │   │   │   ├── test_email.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_email.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_email.cpython-311.pyc
    │   │       │   │   │   ├── test__encoded_words.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test__encoded_words.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test__encoded_words.cpython-311.pyc
    │   │       │   │   │   ├── test_generator.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_generator.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_generator.cpython-311.pyc
    │   │       │   │   │   ├── test_headerregistry.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_headerregistry.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_headerregistry.cpython-311.pyc
    │   │       │   │   │   ├── test__header_value_parser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test__header_value_parser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test__header_value_parser.cpython-311.pyc
    │   │       │   │   │   ├── test_inversion.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_inversion.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_inversion.cpython-311.pyc
    │   │       │   │   │   ├── test_message.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_message.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_message.cpython-311.pyc
    │   │       │   │   │   ├── test_parser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_parser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_parser.cpython-311.pyc
    │   │       │   │   │   ├── test_pickleable.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pickleable.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pickleable.cpython-311.pyc
    │   │       │   │   │   ├── test_policy.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_policy.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_policy.cpython-311.pyc
    │   │       │   │   │   ├── test_utils.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_utils.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_utils.cpython-311.pyc
    │   │       │   │   │   ├── torture_test.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── torture_test.cpython-311.opt-2.pyc
    │   │       │   │   │   └── torture_test.cpython-311.pyc
    │   │       │   │   ├── test_asian_codecs.py
    │   │       │   │   ├── test_contentmanager.py
    │   │       │   │   ├── test_defect_handling.py
    │   │       │   │   ├── test_email.py
    │   │       │   │   ├── test__encoded_words.py
    │   │       │   │   ├── test_generator.py
    │   │       │   │   ├── test_headerregistry.py
    │   │       │   │   ├── test__header_value_parser.py
    │   │       │   │   ├── test_inversion.py
    │   │       │   │   ├── test_message.py
    │   │       │   │   ├── test_parser.py
    │   │       │   │   ├── test_pickleable.py
    │   │       │   │   ├── test_policy.py
    │   │       │   │   ├── test_utils.py
    │   │       │   │   └── torture_test.py
    │   │       │   ├── test_embed.py
    │   │       │   ├── _test_embed_set_config.py
    │   │       │   ├── _test_embed_structseq.py
    │   │       │   ├── test_ensurepip.py
    │   │       │   ├── test_enumerate.py
    │   │       │   ├── test_enum.py
    │   │       │   ├── test_eof.py
    │   │       │   ├── test_epoll.py
    │   │       │   ├── test_errno.py
    │   │       │   ├── test_exception_group.py
    │   │       │   ├── test_exception_hierarchy.py
    │   │       │   ├── test_exceptions.py
    │   │       │   ├── test_exception_variations.py
    │   │       │   ├── test_except_star.py
    │   │       │   ├── test_extcall.py
    │   │       │   ├── test_faulthandler.py
    │   │       │   ├── test_fcntl.py
    │   │       │   ├── test_filecmp.py
    │   │       │   ├── test_file_eintr.py
    │   │       │   ├── test_fileinput.py
    │   │       │   ├── test_fileio.py
    │   │       │   ├── test_file.py
    │   │       │   ├── test_fileutils.py
    │   │       │   ├── test_finalization.py
    │   │       │   ├── test_float.py
    │   │       │   ├── test_flufl.py
    │   │       │   ├── test_fnmatch.py
    │   │       │   ├── test_fork1.py
    │   │       │   ├── test_format.py
    │   │       │   ├── test_fractions.py
    │   │       │   ├── test_frame.py
    │   │       │   ├── test_frozen.py
    │   │       │   ├── test_fstring.py
    │   │       │   ├── test_ftplib.py
    │   │       │   ├── test_funcattrs.py
    │   │       │   ├── test_functools.py
    │   │       │   ├── test_future3.py
    │   │       │   ├── test_future4.py
    │   │       │   ├── test_future5.py
    │   │       │   ├── test___future__.py
    │   │       │   ├── test_future.py
    │   │       │   ├── test_gc.py
    │   │       │   ├── test_gdb.py
    │   │       │   ├── test_generators.py
    │   │       │   ├── test_generator_stop.py
    │   │       │   ├── test_genericalias.py
    │   │       │   ├── test_genericclass.py
    │   │       │   ├── test_genericpath.py
    │   │       │   ├── test_genexps.py
    │   │       │   ├── test_getopt.py
    │   │       │   ├── test_getpass.py
    │   │       │   ├── test_getpath.py
    │   │       │   ├── test_gettext.py
    │   │       │   ├── test_global.py
    │   │       │   ├── test_glob.py
    │   │       │   ├── test_grammar.py
    │   │       │   ├── test_graphlib.py
    │   │       │   ├── test_grp.py
    │   │       │   ├── test_gzip.py
    │   │       │   ├── test_hashlib.py
    │   │       │   ├── test_hash.py
    │   │       │   ├── test_heapq.py
    │   │       │   ├── test_hmac.py
    │   │       │   ├── test_htmlparser.py
    │   │       │   ├── test_html.py
    │   │       │   ├── test_http_cookiejar.py
    │   │       │   ├── test_http_cookies.py
    │   │       │   ├── test_httplib.py
    │   │       │   ├── test_httpservers.py
    │   │       │   ├── test_idle.py
    │   │       │   ├── test_imaplib.py
    │   │       │   ├── test_imghdr.py
    │   │       │   ├── test_import
    │   │       │   │   ├── data
    │   │       │   │   │   ├── circular_imports
    │   │       │   │   │   │   ├── basic2.py
    │   │       │   │   │   │   ├── basic.py
    │   │       │   │   │   │   ├── binding2.py
    │   │       │   │   │   │   ├── binding.py
    │   │       │   │   │   │   ├── from_cycle1.py
    │   │       │   │   │   │   ├── from_cycle2.py
    │   │       │   │   │   │   ├── indirect.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── basic2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── basic2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── basic2.cpython-311.pyc
    │   │       │   │   │   │   │   ├── basic.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── basic.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── basic.cpython-311.pyc
    │   │       │   │   │   │   │   ├── binding2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── binding2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── binding2.cpython-311.pyc
    │   │       │   │   │   │   │   ├── binding.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── binding.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── binding.cpython-311.pyc
    │   │       │   │   │   │   │   ├── from_cycle1.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── from_cycle1.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── from_cycle1.cpython-311.pyc
    │   │       │   │   │   │   │   ├── from_cycle2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── from_cycle2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── from_cycle2.cpython-311.pyc
    │   │       │   │   │   │   │   ├── indirect.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── indirect.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── indirect.cpython-311.pyc
    │   │       │   │   │   │   │   ├── rebinding2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── rebinding2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── rebinding2.cpython-311.pyc
    │   │       │   │   │   │   │   ├── rebinding.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── rebinding.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── rebinding.cpython-311.pyc
    │   │       │   │   │   │   │   ├── source.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── source.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── source.cpython-311.pyc
    │   │       │   │   │   │   │   ├── subpackage.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── subpackage.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── subpackage.cpython-311.pyc
    │   │       │   │   │   │   │   ├── use.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── use.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── use.cpython-311.pyc
    │   │       │   │   │   │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   └── util.cpython-311.pyc
    │   │       │   │   │   │   ├── rebinding2.py
    │   │       │   │   │   │   ├── rebinding.py
    │   │       │   │   │   │   ├── source.py
    │   │       │   │   │   │   ├── subpackage.py
    │   │       │   │   │   │   ├── subpkg
    │   │       │   │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   │   ├── subpackage2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   │   ├── subpackage2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   │   ├── subpackage2.cpython-311.pyc
    │   │       │   │   │   │   │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   │   └── util.cpython-311.pyc
    │   │       │   │   │   │   │   ├── subpackage2.py
    │   │       │   │   │   │   │   └── util.py
    │   │       │   │   │   │   ├── subpkg2
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   ├── parent
    │   │       │   │   │   │   │   │   ├── child.py
    │   │       │   │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │   │       ├── child.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   │       ├── child.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   │       ├── child.cpython-311.pyc
    │   │       │   │   │   │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── use.py
    │   │       │   │   │   │   └── util.py
    │   │       │   │   │   ├── package
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   │   ├── submodule.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── submodule.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   └── submodule.cpython-311.pyc
    │   │       │   │   │   │   └── submodule.py
    │   │       │   │   │   ├── package2
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── submodule1.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── submodule1.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   ├── submodule1.cpython-311.pyc
    │   │       │   │   │   │   │   ├── submodule2.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── submodule2.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   └── submodule2.cpython-311.pyc
    │   │       │   │   │   │   ├── submodule1.py
    │   │       │   │   │   │   └── submodule2.py
    │   │       │   │   │   └── unwritable
    │   │       │   │   │       ├── __init__.py
    │   │       │   │   │       ├── __pycache__
    │   │       │   │   │       │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │       │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │       │   ├── __init__.cpython-311.pyc
    │   │       │   │   │       │   ├── x.cpython-311.opt-1.pyc
    │   │       │   │   │       │   ├── x.cpython-311.opt-2.pyc
    │   │       │   │   │       │   └── x.cpython-311.pyc
    │   │       │   │   │       └── x.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │       └── __main__.cpython-311.pyc
    │   │       │   ├── test_importlib
    │   │       │   │   ├── abc.py
    │   │       │   │   ├── builtin
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_loader.cpython-311.pyc
    │   │       │   │   │   ├── test_finder.py
    │   │       │   │   │   └── test_loader.py
    │   │       │   │   ├── data
    │   │       │   │   │   ├── example2-1.0.0-py3-none-any.whl
    │   │       │   │   │   ├── example-21.12-py3.6.egg
    │   │       │   │   │   ├── example-21.12-py3-none-any.whl
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   └── __pycache__
    │   │       │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   ├── data01
    │   │       │   │   │   ├── binary.file
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   ├── subdirectory
    │   │       │   │   │   │   ├── binary.file
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   └── __pycache__
    │   │       │   │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   ├── utf-16.file
    │   │       │   │   │   └── utf-8.file
    │   │       │   │   ├── data02
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── one
    │   │       │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   ├── __pycache__
    │   │       │   │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   │   └── resource1.txt
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   └── two
    │   │       │   │   │       ├── __init__.py
    │   │       │   │   │       ├── __pycache__
    │   │       │   │   │       │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │       │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │       │   └── __init__.cpython-311.pyc
    │   │       │   │   │       └── resource2.txt
    │   │       │   │   ├── data03
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── namespace
    │   │       │   │   │   │   ├── portion1
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── portion2
    │   │       │   │   │   │   │   ├── __init__.py
    │   │       │   │   │   │   │   └── __pycache__
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   │   │   └── resource1.txt
    │   │       │   │   │   └── __pycache__
    │   │       │   │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │       └── __init__.cpython-311.pyc
    │   │       │   │   ├── extension
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.pyc
    │   │       │   │   │   │   ├── test_path_hook.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_path_hook.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_path_hook.cpython-311.pyc
    │   │       │   │   │   ├── test_case_sensitivity.py
    │   │       │   │   │   ├── test_finder.py
    │   │       │   │   │   ├── test_loader.py
    │   │       │   │   │   └── test_path_hook.py
    │   │       │   │   ├── fixtures.py
    │   │       │   │   ├── frozen
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_loader.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_loader.cpython-311.pyc
    │   │       │   │   │   ├── test_finder.py
    │   │       │   │   │   └── test_loader.py
    │   │       │   │   ├── import_
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_api.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_api.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_api.cpython-311.pyc
    │   │       │   │   │   │   ├── test_caching.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_caching.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_caching.cpython-311.pyc
    │   │       │   │   │   │   ├── test_fromlist.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_fromlist.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_fromlist.cpython-311.pyc
    │   │       │   │   │   │   ├── test___loader__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test___loader__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test___loader__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_meta_path.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_meta_path.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_meta_path.cpython-311.pyc
    │   │       │   │   │   │   ├── test___package__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test___package__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test___package__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_packages.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_packages.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_packages.cpython-311.pyc
    │   │       │   │   │   │   ├── test_path.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_path.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_path.cpython-311.pyc
    │   │       │   │   │   │   ├── test_relative_imports.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_relative_imports.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_relative_imports.cpython-311.pyc
    │   │       │   │   │   ├── test_api.py
    │   │       │   │   │   ├── test_caching.py
    │   │       │   │   │   ├── test_fromlist.py
    │   │       │   │   │   ├── test___loader__.py
    │   │       │   │   │   ├── test_meta_path.py
    │   │       │   │   │   ├── test___package__.py
    │   │       │   │   │   ├── test_packages.py
    │   │       │   │   │   ├── test_path.py
    │   │       │   │   │   └── test_relative_imports.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── namespacedata01
    │   │       │   │   │   ├── binary.file
    │   │       │   │   │   ├── utf-16.file
    │   │       │   │   │   └── utf-8.file
    │   │       │   │   ├── namespace_pkgs
    │   │       │   │   │   ├── both_portions
    │   │       │   │   │   │   └── foo
    │   │       │   │   │   │       ├── one.py
    │   │       │   │   │   │       ├── __pycache__
    │   │       │   │   │   │       │   ├── one.cpython-311.opt-1.pyc
    │   │       │   │   │   │       │   ├── one.cpython-311.opt-2.pyc
    │   │       │   │   │   │       │   ├── one.cpython-311.pyc
    │   │       │   │   │   │       │   ├── two.cpython-311.opt-1.pyc
    │   │       │   │   │   │       │   ├── two.cpython-311.opt-2.pyc
    │   │       │   │   │   │       │   └── two.cpython-311.pyc
    │   │       │   │   │   │       └── two.py
    │   │       │   │   │   ├── missing_directory.zip
    │   │       │   │   │   ├── module_and_namespace_package
    │   │       │   │   │   │   ├── a_test
    │   │       │   │   │   │   │   └── empty
    │   │       │   │   │   │   ├── a_test.py
    │   │       │   │   │   │   └── __pycache__
    │   │       │   │   │   │       ├── a_test.cpython-311.opt-1.pyc
    │   │       │   │   │   │       ├── a_test.cpython-311.opt-2.pyc
    │   │       │   │   │   │       └── a_test.cpython-311.pyc
    │   │       │   │   │   ├── nested_portion1.zip
    │   │       │   │   │   ├── not_a_namespace_pkg
    │   │       │   │   │   │   └── foo
    │   │       │   │   │   │       ├── __init__.py
    │   │       │   │   │   │       ├── one.py
    │   │       │   │   │   │       └── __pycache__
    │   │       │   │   │   │           ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │           ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │           ├── __init__.cpython-311.pyc
    │   │       │   │   │   │           ├── one.cpython-311.opt-1.pyc
    │   │       │   │   │   │           ├── one.cpython-311.opt-2.pyc
    │   │       │   │   │   │           └── one.cpython-311.pyc
    │   │       │   │   │   ├── portion1
    │   │       │   │   │   │   └── foo
    │   │       │   │   │   │       ├── one.py
    │   │       │   │   │   │       └── __pycache__
    │   │       │   │   │   │           ├── one.cpython-311.opt-1.pyc
    │   │       │   │   │   │           ├── one.cpython-311.opt-2.pyc
    │   │       │   │   │   │           └── one.cpython-311.pyc
    │   │       │   │   │   ├── portion2
    │   │       │   │   │   │   └── foo
    │   │       │   │   │   │       ├── __pycache__
    │   │       │   │   │   │       │   ├── two.cpython-311.opt-1.pyc
    │   │       │   │   │   │       │   ├── two.cpython-311.opt-2.pyc
    │   │       │   │   │   │       │   └── two.cpython-311.pyc
    │   │       │   │   │   │       └── two.py
    │   │       │   │   │   ├── project1
    │   │       │   │   │   │   └── parent
    │   │       │   │   │   │       └── child
    │   │       │   │   │   │           ├── one.py
    │   │       │   │   │   │           └── __pycache__
    │   │       │   │   │   │               ├── one.cpython-311.opt-1.pyc
    │   │       │   │   │   │               ├── one.cpython-311.opt-2.pyc
    │   │       │   │   │   │               └── one.cpython-311.pyc
    │   │       │   │   │   ├── project2
    │   │       │   │   │   │   └── parent
    │   │       │   │   │   │       └── child
    │   │       │   │   │   │           ├── __pycache__
    │   │       │   │   │   │           │   ├── two.cpython-311.opt-1.pyc
    │   │       │   │   │   │           │   ├── two.cpython-311.opt-2.pyc
    │   │       │   │   │   │           │   └── two.cpython-311.pyc
    │   │       │   │   │   │           └── two.py
    │   │       │   │   │   ├── project3
    │   │       │   │   │   │   └── parent
    │   │       │   │   │   │       └── child
    │   │       │   │   │   │           ├── __pycache__
    │   │       │   │   │   │           │   ├── three.cpython-311.opt-1.pyc
    │   │       │   │   │   │           │   ├── three.cpython-311.opt-2.pyc
    │   │       │   │   │   │           │   └── three.cpython-311.pyc
    │   │       │   │   │   │           └── three.py
    │   │       │   │   │   └── top_level_portion1.zip
    │   │       │   │   ├── partial
    │   │       │   │   │   ├── cfimport.py
    │   │       │   │   │   ├── pool_in_threads.py
    │   │       │   │   │   └── __pycache__
    │   │       │   │   │       ├── cfimport.cpython-311.opt-1.pyc
    │   │       │   │   │       ├── cfimport.cpython-311.opt-2.pyc
    │   │       │   │   │       ├── cfimport.cpython-311.pyc
    │   │       │   │   │       ├── pool_in_threads.cpython-311.opt-1.pyc
    │   │       │   │   │       ├── pool_in_threads.cpython-311.opt-2.pyc
    │   │       │   │   │       └── pool_in_threads.cpython-311.pyc
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── abc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── abc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── abc.cpython-311.pyc
    │   │       │   │   │   ├── fixtures.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── fixtures.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── fixtures.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── stubs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── stubs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── stubs.cpython-311.pyc
    │   │       │   │   │   ├── test_abc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_abc.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_abc.cpython-311.pyc
    │   │       │   │   │   ├── test_api.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_api.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_api.cpython-311.pyc
    │   │       │   │   │   ├── test_compatibilty_files.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_compatibilty_files.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_compatibilty_files.cpython-311.pyc
    │   │       │   │   │   ├── test_contents.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_contents.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_contents.cpython-311.pyc
    │   │       │   │   │   ├── test_files.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_files.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_files.cpython-311.pyc
    │   │       │   │   │   ├── test_lazy.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_lazy.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_lazy.cpython-311.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_locks.cpython-311.pyc
    │   │       │   │   │   ├── test_main.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_main.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_main.cpython-311.pyc
    │   │       │   │   │   ├── test_metadata_api.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_metadata_api.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_metadata_api.cpython-311.pyc
    │   │       │   │   │   ├── test_namespace_pkgs.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_namespace_pkgs.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_namespace_pkgs.cpython-311.pyc
    │   │       │   │   │   ├── test_open.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_open.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_open.cpython-311.pyc
    │   │       │   │   │   ├── test_path.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_path.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_path.cpython-311.pyc
    │   │       │   │   │   ├── test_pkg_import.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pkg_import.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pkg_import.cpython-311.pyc
    │   │       │   │   │   ├── test_read.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_read.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_read.cpython-311.pyc
    │   │       │   │   │   ├── test_reader.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_reader.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_reader.cpython-311.pyc
    │   │       │   │   │   ├── test_resource.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_resource.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_resource.cpython-311.pyc
    │   │       │   │   │   ├── test_spec.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_spec.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_spec.cpython-311.pyc
    │   │       │   │   │   ├── test_threaded_import.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_threaded_import.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_threaded_import.cpython-311.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_util.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_util.cpython-311.pyc
    │   │       │   │   │   ├── test_windows.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_windows.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_windows.cpython-311.pyc
    │   │       │   │   │   ├── test_zip.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_zip.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_zip.cpython-311.pyc
    │   │       │   │   │   ├── threaded_import_hangers.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── threaded_import_hangers.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── threaded_import_hangers.cpython-311.pyc
    │   │       │   │   │   ├── update-zips.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── update-zips.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── update-zips.cpython-311.pyc
    │   │       │   │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   │   └── util.cpython-311.pyc
    │   │       │   │   ├── resources
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── util.cpython-311.pyc
    │   │       │   │   │   └── util.py
    │   │       │   │   ├── source
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_case_sensitivity.cpython-311.pyc
    │   │       │   │   │   │   ├── test_file_loader.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_file_loader.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_file_loader.cpython-311.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_finder.cpython-311.pyc
    │   │       │   │   │   │   ├── test_path_hook.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_path_hook.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_path_hook.cpython-311.pyc
    │   │       │   │   │   │   ├── test_source_encoding.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_source_encoding.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_source_encoding.cpython-311.pyc
    │   │       │   │   │   ├── test_case_sensitivity.py
    │   │       │   │   │   ├── test_file_loader.py
    │   │       │   │   │   ├── test_finder.py
    │   │       │   │   │   ├── test_path_hook.py
    │   │       │   │   │   └── test_source_encoding.py
    │   │       │   │   ├── stubs.py
    │   │       │   │   ├── test_abc.py
    │   │       │   │   ├── test_api.py
    │   │       │   │   ├── test_compatibilty_files.py
    │   │       │   │   ├── test_contents.py
    │   │       │   │   ├── test_files.py
    │   │       │   │   ├── test_lazy.py
    │   │       │   │   ├── test_locks.py
    │   │       │   │   ├── test_main.py
    │   │       │   │   ├── test_metadata_api.py
    │   │       │   │   ├── test_namespace_pkgs.py
    │   │       │   │   ├── test_open.py
    │   │       │   │   ├── test_path.py
    │   │       │   │   ├── test_pkg_import.py
    │   │       │   │   ├── test_reader.py
    │   │       │   │   ├── test_read.py
    │   │       │   │   ├── test_resource.py
    │   │       │   │   ├── test_spec.py
    │   │       │   │   ├── test_threaded_import.py
    │   │       │   │   ├── test_util.py
    │   │       │   │   ├── test_windows.py
    │   │       │   │   ├── test_zip.py
    │   │       │   │   ├── threaded_import_hangers.py
    │   │       │   │   ├── update-zips.py
    │   │       │   │   ├── util.py
    │   │       │   │   ├── zipdata01
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── __init__.cpython-311.pyc
    │   │       │   │   │   └── ziptestdata.zip
    │   │       │   │   └── zipdata02
    │   │       │   │       ├── __init__.py
    │   │       │   │       ├── __pycache__
    │   │       │   │       │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       │   └── __init__.cpython-311.pyc
    │   │       │   │       └── ziptestdata.zip
    │   │       │   ├── test_imp.py
    │   │       │   ├── test_index.py
    │   │       │   ├── test_inspect.py
    │   │       │   ├── test_interpreters.py
    │   │       │   ├── test_int_literal.py
    │   │       │   ├── test_int.py
    │   │       │   ├── test_ioctl.py
    │   │       │   ├── test_io.py
    │   │       │   ├── test_ipaddress.py
    │   │       │   ├── test_isinstance.py
    │   │       │   ├── test_iterlen.py
    │   │       │   ├── test_iter.py
    │   │       │   ├── test_itertools.py
    │   │       │   ├── test_json
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_decode.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_decode.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_decode.cpython-311.pyc
    │   │       │   │   │   ├── test_default.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_default.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_default.cpython-311.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.pyc
    │   │       │   │   │   ├── test_encode_basestring_ascii.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_encode_basestring_ascii.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_encode_basestring_ascii.cpython-311.pyc
    │   │       │   │   │   ├── test_enum.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_enum.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_enum.cpython-311.pyc
    │   │       │   │   │   ├── test_fail.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_fail.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_fail.cpython-311.pyc
    │   │       │   │   │   ├── test_float.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_float.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_float.cpython-311.pyc
    │   │       │   │   │   ├── test_indent.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_indent.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_indent.cpython-311.pyc
    │   │       │   │   │   ├── test_pass1.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pass1.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pass1.cpython-311.pyc
    │   │       │   │   │   ├── test_pass2.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pass2.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pass2.cpython-311.pyc
    │   │       │   │   │   ├── test_pass3.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pass3.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pass3.cpython-311.pyc
    │   │       │   │   │   ├── test_recursion.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_recursion.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_recursion.cpython-311.pyc
    │   │       │   │   │   ├── test_scanstring.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_scanstring.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_scanstring.cpython-311.pyc
    │   │       │   │   │   ├── test_separators.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_separators.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_separators.cpython-311.pyc
    │   │       │   │   │   ├── test_speedups.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_speedups.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_speedups.cpython-311.pyc
    │   │       │   │   │   ├── test_tool.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_tool.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_tool.cpython-311.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_unicode.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_unicode.cpython-311.pyc
    │   │       │   │   ├── test_decode.py
    │   │       │   │   ├── test_default.py
    │   │       │   │   ├── test_dump.py
    │   │       │   │   ├── test_encode_basestring_ascii.py
    │   │       │   │   ├── test_enum.py
    │   │       │   │   ├── test_fail.py
    │   │       │   │   ├── test_float.py
    │   │       │   │   ├── test_indent.py
    │   │       │   │   ├── test_pass1.py
    │   │       │   │   ├── test_pass2.py
    │   │       │   │   ├── test_pass3.py
    │   │       │   │   ├── test_recursion.py
    │   │       │   │   ├── test_scanstring.py
    │   │       │   │   ├── test_separators.py
    │   │       │   │   ├── test_speedups.py
    │   │       │   │   ├── test_tool.py
    │   │       │   │   └── test_unicode.py
    │   │       │   ├── test_keywordonlyarg.py
    │   │       │   ├── test_keyword.py
    │   │       │   ├── test_kqueue.py
    │   │       │   ├── test_largefile.py
    │   │       │   ├── test_launcher.py
    │   │       │   ├── test_lib2to3.py
    │   │       │   ├── test_linecache.py
    │   │       │   ├── test_listcomps.py
    │   │       │   ├── test_list.py
    │   │       │   ├── test_lltrace.py
    │   │       │   ├── test__locale.py
    │   │       │   ├── test_locale.py
    │   │       │   ├── test_logging.py
    │   │       │   ├── test_longexp.py
    │   │       │   ├── test_long.py
    │   │       │   ├── test_lzma.py
    │   │       │   ├── test_mailbox.py
    │   │       │   ├── test_mailcap.py
    │   │       │   ├── test_marshal.py
    │   │       │   ├── test_math.py
    │   │       │   ├── test_memoryio.py
    │   │       │   ├── test_memoryview.py
    │   │       │   ├── test_metaclass.py
    │   │       │   ├── test_mimetypes.py
    │   │       │   ├── test_minidom.py
    │   │       │   ├── test_mmap.py
    │   │       │   ├── test_modulefinder.py
    │   │       │   ├── test_module.py
    │   │       │   ├── test_msilib.py
    │   │       │   ├── test_multibytecodec.py
    │   │       │   ├── test_multiprocessing_fork.py
    │   │       │   ├── test_multiprocessing_forkserver.py
    │   │       │   ├── test_multiprocessing_main_handling.py
    │   │       │   ├── _test_multiprocessing.py
    │   │       │   ├── test_multiprocessing_spawn.py
    │   │       │   ├── test_named_expressions.py
    │   │       │   ├── test_netrc.py
    │   │       │   ├── test_nis.py
    │   │       │   ├── test_nntplib.py
    │   │       │   ├── test_ntpath.py
    │   │       │   ├── test_numeric_tower.py
    │   │       │   ├── test_opcache.py
    │   │       │   ├── test__opcode.py
    │   │       │   ├── test_opcodes.py
    │   │       │   ├── test_openpty.py
    │   │       │   ├── test_operator.py
    │   │       │   ├── test_optparse.py
    │   │       │   ├── test_ordered_dict.py
    │   │       │   ├── test_os.py
    │   │       │   ├── test_ossaudiodev.py
    │   │       │   ├── test_osx_env.py
    │   │       │   ├── test__osx_support.py
    │   │       │   ├── test_pathlib.py
    │   │       │   ├── test_patma.py
    │   │       │   ├── test_pdb.py
    │   │       │   ├── test_peepholer.py
    │   │       │   ├── test_peg_generator
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_c_parser.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_c_parser.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_c_parser.cpython-311.pyc
    │   │       │   │   │   ├── test_first_sets.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_first_sets.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_first_sets.cpython-311.pyc
    │   │       │   │   │   ├── test_grammar_validator.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_grammar_validator.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_grammar_validator.cpython-311.pyc
    │   │       │   │   │   ├── test_pegen.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pegen.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_pegen.cpython-311.pyc
    │   │       │   │   ├── test_c_parser.py
    │   │       │   │   ├── test_first_sets.py
    │   │       │   │   ├── test_grammar_validator.py
    │   │       │   │   └── test_pegen.py
    │   │       │   ├── test_pep646_syntax.py
    │   │       │   ├── test_picklebuffer.py
    │   │       │   ├── test_pickle.py
    │   │       │   ├── test_pickletools.py
    │   │       │   ├── test_pipes.py
    │   │       │   ├── test_pkg.py
    │   │       │   ├── test_pkgutil.py
    │   │       │   ├── test_platform.py
    │   │       │   ├── test_plistlib.py
    │   │       │   ├── test_poll.py
    │   │       │   ├── test_popen.py
    │   │       │   ├── test_poplib.py
    │   │       │   ├── test_positional_only_arg.py
    │   │       │   ├── test_posixpath.py
    │   │       │   ├── test_posix.py
    │   │       │   ├── test_pow.py
    │   │       │   ├── test_pprint.py
    │   │       │   ├── test_print.py
    │   │       │   ├── test_profile.py
    │   │       │   ├── test_property.py
    │   │       │   ├── test_pstats.py
    │   │       │   ├── test_pty.py
    │   │       │   ├── test_pulldom.py
    │   │       │   ├── test_pwd.py
    │   │       │   ├── test_pyclbr.py
    │   │       │   ├── test_py_compile.py
    │   │       │   ├── test_pydoc.py
    │   │       │   ├── test_pyexpat.py
    │   │       │   ├── test_queue.py
    │   │       │   ├── test_quopri.py
    │   │       │   ├── test_raise.py
    │   │       │   ├── test_random.py
    │   │       │   ├── test_range.py
    │   │       │   ├── test_readline.py
    │   │       │   ├── test_regrtest.py
    │   │       │   ├── test_repl.py
    │   │       │   ├── test_reprlib.py
    │   │       │   ├── test_re.py
    │   │       │   ├── test_resource.py
    │   │       │   ├── test_richcmp.py
    │   │       │   ├── test_rlcompleter.py
    │   │       │   ├── test_robotparser.py
    │   │       │   ├── test_runpy.py
    │   │       │   ├── test_sax.py
    │   │       │   ├── test_sched.py
    │   │       │   ├── test_scope.py
    │   │       │   ├── test_script_helper.py
    │   │       │   ├── test_secrets.py
    │   │       │   ├── test_selectors.py
    │   │       │   ├── test_select.py
    │   │       │   ├── test_setcomps.py
    │   │       │   ├── test_set.py
    │   │       │   ├── test_shelve.py
    │   │       │   ├── test_shlex.py
    │   │       │   ├── test_shutil.py
    │   │       │   ├── test_signal.py
    │   │       │   ├── test_site.py
    │   │       │   ├── test_slice.py
    │   │       │   ├── test_smtpd.py
    │   │       │   ├── test_smtplib.py
    │   │       │   ├── test_smtpnet.py
    │   │       │   ├── test_sndhdr.py
    │   │       │   ├── test_socket.py
    │   │       │   ├── test_socketserver.py
    │   │       │   ├── test_sort.py
    │   │       │   ├── test_source_encoding.py
    │   │       │   ├── test_spwd.py
    │   │       │   ├── test_sqlite3
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_backup.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_backup.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_backup.cpython-311.pyc
    │   │       │   │   │   ├── test_dbapi.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dbapi.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dbapi.cpython-311.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_dump.cpython-311.pyc
    │   │       │   │   │   ├── test_factory.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_factory.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_factory.cpython-311.pyc
    │   │       │   │   │   ├── test_hooks.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_hooks.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_hooks.cpython-311.pyc
    │   │       │   │   │   ├── test_regression.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_regression.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_regression.cpython-311.pyc
    │   │       │   │   │   ├── test_transactions.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_transactions.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_transactions.cpython-311.pyc
    │   │       │   │   │   ├── test_types.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_types.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_types.cpython-311.pyc
    │   │       │   │   │   ├── test_userfunctions.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_userfunctions.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_userfunctions.cpython-311.pyc
    │   │       │   │   ├── test_backup.py
    │   │       │   │   ├── test_dbapi.py
    │   │       │   │   ├── test_dump.py
    │   │       │   │   ├── test_factory.py
    │   │       │   │   ├── test_hooks.py
    │   │       │   │   ├── test_regression.py
    │   │       │   │   ├── test_transactions.py
    │   │       │   │   ├── test_types.py
    │   │       │   │   └── test_userfunctions.py
    │   │       │   ├── test_ssl.py
    │   │       │   ├── test_stable_abi_ctypes.py
    │   │       │   ├── test_startfile.py
    │   │       │   ├── test_statistics.py
    │   │       │   ├── test_stat.py
    │   │       │   ├── test_strftime.py
    │   │       │   ├── test_string_literals.py
    │   │       │   ├── test_stringprep.py
    │   │       │   ├── test_string.py
    │   │       │   ├── test_strptime.py
    │   │       │   ├── test_strtod.py
    │   │       │   ├── test_struct.py
    │   │       │   ├── test_structseq.py
    │   │       │   ├── test_subclassinit.py
    │   │       │   ├── test_subprocess.py
    │   │       │   ├── test_sunau.py
    │   │       │   ├── test_sundry.py
    │   │       │   ├── test_super.py
    │   │       │   ├── test_support.py
    │   │       │   ├── test_symtable.py
    │   │       │   ├── test_syntax.py
    │   │       │   ├── test_sysconfig.py
    │   │       │   ├── test_syslog.py
    │   │       │   ├── test_sys.py
    │   │       │   ├── test_sys_setprofile.py
    │   │       │   ├── test_sys_settrace.py
    │   │       │   ├── test_tabnanny.py
    │   │       │   ├── test_tarfile.py
    │   │       │   ├── testtar.tar
    │   │       │   ├── testtar.tar.xz
    │   │       │   ├── test_tcl.py
    │   │       │   ├── test_telnetlib.py
    │   │       │   ├── test_tempfile.py
    │   │       │   ├── test_textwrap.py
    │   │       │   ├── test_threadedtempfile.py
    │   │       │   ├── test_threading_local.py
    │   │       │   ├── test_threading.py
    │   │       │   ├── test_thread.py
    │   │       │   ├── test_threadsignals.py
    │   │       │   ├── test_timeit.py
    │   │       │   ├── test_timeout.py
    │   │       │   ├── test_time.py
    │   │       │   ├── test_tix.py
    │   │       │   ├── test_tk.py
    │   │       │   ├── test_tokenize.py
    │   │       │   ├── test_tomllib
    │   │       │   │   ├── burntsushi.py
    │   │       │   │   ├── data
    │   │       │   │   │   ├── invalid
    │   │       │   │   │   │   ├── array
    │   │       │   │   │   │   │   ├── file-end-after-val.toml
    │   │       │   │   │   │   │   ├── unclosed-after-item.toml
    │   │       │   │   │   │   │   └── unclosed-empty.toml
    │   │       │   │   │   │   ├── array-missing-comma.toml
    │   │       │   │   │   │   ├── array-of-tables
    │   │       │   │   │   │   │   ├── overwrite-array-in-parent.toml
    │   │       │   │   │   │   │   └── overwrite-bool-with-aot.toml
    │   │       │   │   │   │   ├── basic-str-ends-in-escape.toml
    │   │       │   │   │   │   ├── boolean
    │   │       │   │   │   │   │   ├── invalid-false-casing.toml
    │   │       │   │   │   │   │   └── invalid-true-casing.toml
    │   │       │   │   │   │   ├── dates-and-times
    │   │       │   │   │   │   │   └── invalid-day.toml
    │   │       │   │   │   │   ├── dotted-keys
    │   │       │   │   │   │   │   ├── access-non-table.toml
    │   │       │   │   │   │   │   ├── extend-defined-aot.toml
    │   │       │   │   │   │   │   ├── extend-defined-table.toml
    │   │       │   │   │   │   │   └── extend-defined-table-with-subtable.toml
    │   │       │   │   │   │   ├── inline-table
    │   │       │   │   │   │   │   ├── define-twice-in-subtable.toml
    │   │       │   │   │   │   │   ├── define-twice.toml
    │   │       │   │   │   │   │   ├── file-end-after-key-val.toml
    │   │       │   │   │   │   │   ├── mutate.toml
    │   │       │   │   │   │   │   ├── override-val-in-table.toml
    │   │       │   │   │   │   │   ├── override-val-with-array.toml
    │   │       │   │   │   │   │   ├── override-val-with-table.toml
    │   │       │   │   │   │   │   ├── overwrite-implicitly.toml
    │   │       │   │   │   │   │   ├── overwrite-value-in-inner-array.toml
    │   │       │   │   │   │   │   ├── overwrite-value-in-inner-table.toml
    │   │       │   │   │   │   │   └── unclosed-empty.toml
    │   │       │   │   │   │   ├── inline-table-missing-comma.toml
    │   │       │   │   │   │   ├── invalid-comment-char.toml
    │   │       │   │   │   │   ├── invalid-escaped-unicode.toml
    │   │       │   │   │   │   ├── invalid-hex.toml
    │   │       │   │   │   │   ├── keys-and-vals
    │   │       │   │   │   │   │   ├── ends-early-table-def.toml
    │   │       │   │   │   │   │   ├── ends-early.toml
    │   │       │   │   │   │   │   ├── no-value.toml
    │   │       │   │   │   │   │   ├── only-ws-after-dot.toml
    │   │       │   │   │   │   │   └── overwrite-with-deep-table.toml
    │   │       │   │   │   │   ├── literal-str
    │   │       │   │   │   │   │   └── unclosed.toml
    │   │       │   │   │   │   ├── missing-closing-double-square-bracket.toml
    │   │       │   │   │   │   ├── missing-closing-square-bracket.toml
    │   │       │   │   │   │   ├── multiline-basic-str
    │   │       │   │   │   │   │   ├── carriage-return.toml
    │   │       │   │   │   │   │   ├── escape-only.toml
    │   │       │   │   │   │   │   ├── file-ends-after-opening.toml
    │   │       │   │   │   │   │   ├── last-line-escape.toml
    │   │       │   │   │   │   │   └── unclosed-ends-in-whitespace-escape.toml
    │   │       │   │   │   │   ├── multiline-literal-str
    │   │       │   │   │   │   │   ├── file-ends-after-opening.toml
    │   │       │   │   │   │   │   └── unclosed.toml
    │   │       │   │   │   │   ├── non-scalar-escaped.toml
    │   │       │   │   │   │   ├── table
    │   │       │   │   │   │   │   ├── eof-after-opening.toml
    │   │       │   │   │   │   │   ├── redefine-1.toml
    │   │       │   │   │   │   │   └── redefine-2.toml
    │   │       │   │   │   │   ├── unclosed-multiline-string.toml
    │   │       │   │   │   │   └── unclosed-string.toml
    │   │       │   │   │   └── valid
    │   │       │   │   │       ├── apostrophes-in-literal-string.json
    │   │       │   │   │       ├── apostrophes-in-literal-string.toml
    │   │       │   │   │       ├── array
    │   │       │   │   │       │   ├── array-subtables.json
    │   │       │   │   │       │   ├── array-subtables.toml
    │   │       │   │   │       │   ├── open-parent-table.json
    │   │       │   │   │       │   └── open-parent-table.toml
    │   │       │   │   │       ├── boolean.json
    │   │       │   │   │       ├── boolean.toml
    │   │       │   │   │       ├── dates-and-times
    │   │       │   │   │       │   ├── datetimes.json
    │   │       │   │   │       │   ├── datetimes.toml
    │   │       │   │   │       │   ├── localtime.json
    │   │       │   │   │       │   └── localtime.toml
    │   │       │   │   │       ├── empty-inline-table.json
    │   │       │   │   │       ├── empty-inline-table.toml
    │   │       │   │   │       ├── five-quotes.json
    │   │       │   │   │       ├── five-quotes.toml
    │   │       │   │   │       ├── hex-char.json
    │   │       │   │   │       ├── hex-char.toml
    │   │       │   │   │       ├── multiline-basic-str
    │   │       │   │   │       │   ├── ends-in-whitespace-escape.json
    │   │       │   │   │       │   └── ends-in-whitespace-escape.toml
    │   │       │   │   │       ├── no-newlines.json
    │   │       │   │   │       ├── no-newlines.toml
    │   │       │   │   │       ├── trailing-comma.json
    │   │       │   │   │       └── trailing-comma.toml
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── burntsushi.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── burntsushi.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── burntsushi.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_data.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_data.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_data.cpython-311.pyc
    │   │       │   │   │   ├── test_error.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_error.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_error.cpython-311.pyc
    │   │       │   │   │   ├── test_misc.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_misc.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_misc.cpython-311.pyc
    │   │       │   │   ├── test_data.py
    │   │       │   │   ├── test_error.py
    │   │       │   │   └── test_misc.py
    │   │       │   ├── test_tools
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── test_fixcid.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_fixcid.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_fixcid.cpython-311.pyc
    │   │       │   │   │   ├── test_freeze.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_freeze.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_freeze.cpython-311.pyc
    │   │       │   │   │   ├── test_gprof2html.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_gprof2html.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_gprof2html.cpython-311.pyc
    │   │       │   │   │   ├── test_i18n.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_i18n.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_i18n.cpython-311.pyc
    │   │       │   │   │   ├── test_lll.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_lll.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_lll.cpython-311.pyc
    │   │       │   │   │   ├── test_md5sum.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_md5sum.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_md5sum.cpython-311.pyc
    │   │       │   │   │   ├── test_pathfix.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pathfix.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pathfix.cpython-311.pyc
    │   │       │   │   │   ├── test_pdeps.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pdeps.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pdeps.cpython-311.pyc
    │   │       │   │   │   ├── test_pindent.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_pindent.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_pindent.cpython-311.pyc
    │   │       │   │   │   ├── test_reindent.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_reindent.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_reindent.cpython-311.pyc
    │   │       │   │   │   ├── test_sundry.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_sundry.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_sundry.cpython-311.pyc
    │   │       │   │   ├── test_fixcid.py
    │   │       │   │   ├── test_freeze.py
    │   │       │   │   ├── test_gprof2html.py
    │   │       │   │   ├── test_i18n.py
    │   │       │   │   ├── test_lll.py
    │   │       │   │   ├── test_md5sum.py
    │   │       │   │   ├── test_pathfix.py
    │   │       │   │   ├── test_pdeps.py
    │   │       │   │   ├── test_pindent.py
    │   │       │   │   ├── test_reindent.py
    │   │       │   │   └── test_sundry.py
    │   │       │   ├── test_traceback.py
    │   │       │   ├── test_tracemalloc.py
    │   │       │   ├── test_trace.py
    │   │       │   ├── test_ttk_guionly.py
    │   │       │   ├── test_ttk_textonly.py
    │   │       │   ├── test_tuple.py
    │   │       │   ├── test_turtle.py
    │   │       │   ├── test_type_annotations.py
    │   │       │   ├── test_type_cache.py
    │   │       │   ├── test_typechecks.py
    │   │       │   ├── test_type_comments.py
    │   │       │   ├── test_types.py
    │   │       │   ├── test_typing.py
    │   │       │   ├── test_ucn.py
    │   │       │   ├── test_unary.py
    │   │       │   ├── test_unicodedata.py
    │   │       │   ├── test_unicode_file_functions.py
    │   │       │   ├── test_unicode_file.py
    │   │       │   ├── test_unicode_identifiers.py
    │   │       │   ├── test_unicode.py
    │   │       │   ├── test_unittest.py
    │   │       │   ├── test_univnewlines.py
    │   │       │   ├── test_unpack_ex.py
    │   │       │   ├── test_unpack.py
    │   │       │   ├── test_unparse.py
    │   │       │   ├── test_urllib2_localnet.py
    │   │       │   ├── test_urllib2net.py
    │   │       │   ├── test_urllib2.py
    │   │       │   ├── test_urllibnet.py
    │   │       │   ├── test_urllib.py
    │   │       │   ├── test_urllib_response.py
    │   │       │   ├── test_urlparse.py
    │   │       │   ├── test_userdict.py
    │   │       │   ├── test_userlist.py
    │   │       │   ├── test_userstring.py
    │   │       │   ├── test_utf8_mode.py
    │   │       │   ├── test_utf8source.py
    │   │       │   ├── test_uuid.py
    │   │       │   ├── test_uu.py
    │   │       │   ├── _test_venv_multiprocessing.py
    │   │       │   ├── test_venv.py
    │   │       │   ├── test_wait3.py
    │   │       │   ├── test_wait4.py
    │   │       │   ├── test_warnings
    │   │       │   │   ├── data
    │   │       │   │   │   ├── import_warning.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── import_warning.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── import_warning.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── import_warning.cpython-311.pyc
    │   │       │   │   │   │   ├── stacklevel.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── stacklevel.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── stacklevel.cpython-311.pyc
    │   │       │   │   │   └── stacklevel.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       ├── __init__.cpython-311.pyc
    │   │       │   │       ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │       └── __main__.cpython-311.pyc
    │   │       │   ├── test_wave.py
    │   │       │   ├── test_weakref.py
    │   │       │   ├── test_weakset.py
    │   │       │   ├── test_webbrowser.py
    │   │       │   ├── test_winconsoleio.py
    │   │       │   ├── test_winreg.py
    │   │       │   ├── test_winsound.py
    │   │       │   ├── test_with.py
    │   │       │   ├── test_wsgiref.py
    │   │       │   ├── test_xdrlib.py
    │   │       │   ├── test_xml_dom_minicompat.py
    │   │       │   ├── test_xml_etree_c.py
    │   │       │   ├── test_xml_etree.py
    │   │       │   ├── test_xmlrpc_net.py
    │   │       │   ├── test_xmlrpc.py
    │   │       │   ├── test_xxlimited.py
    │   │       │   ├── test__xxsubinterpreters.py
    │   │       │   ├── test_xxtestfuzz.py
    │   │       │   ├── test_yield_from.py
    │   │       │   ├── test_zipapp.py
    │   │       │   ├── test_zipfile64.py
    │   │       │   ├── test_zipfile.py
    │   │       │   ├── test_zipimport.py
    │   │       │   ├── test_zipimport_support.py
    │   │       │   ├── test_zlib.py
    │   │       │   ├── test_zoneinfo
    │   │       │   │   ├── data
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── update_test_data.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── update_test_data.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── update_test_data.cpython-311.pyc
    │   │       │   │   │   ├── update_test_data.py
    │   │       │   │   │   └── zoneinfo_data.json
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── _support.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _support.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── _support.cpython-311.pyc
    │   │       │   │   │   ├── test_zoneinfo.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_zoneinfo.cpython-311.opt-2.pyc
    │   │       │   │   │   └── test_zoneinfo.cpython-311.pyc
    │   │       │   │   ├── _support.py
    │   │       │   │   └── test_zoneinfo.py
    │   │       │   ├── tf_inherit_check.py
    │   │       │   ├── time_hashlib.py
    │   │       │   ├── tokenize_tests-latin1-coding-cookie-and-utf8-bom-sig.txt
    │   │       │   ├── tokenize_tests-no-coding-cookie-and-utf8-bom-sig-only.txt
    │   │       │   ├── tokenize_tests.txt
    │   │       │   ├── tokenize_tests-utf8-coding-cookie-and-no-utf8-bom-sig.txt
    │   │       │   ├── tokenize_tests-utf8-coding-cookie-and-utf8-bom-sig.txt
    │   │       │   ├── tracedmodules
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── testmod.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── testmod.cpython-311.opt-2.pyc
    │   │       │   │   │   └── testmod.cpython-311.pyc
    │   │       │   │   └── testmod.py
    │   │       │   ├── _typed_dict_helper.py
    │   │       │   ├── typinganndata
    │   │       │   │   ├── ann_module9.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── ann_module9.cpython-311.opt-1.pyc
    │   │       │   │       ├── ann_module9.cpython-311.opt-2.pyc
    │   │       │   │       ├── ann_module9.cpython-311.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   ├── win_console_handler.py
    │   │       │   ├── xmltestdata
    │   │       │   │   ├── c14n-20
    │   │       │   │   │   ├── c14nComment.xml
    │   │       │   │   │   ├── c14nDefault.xml
    │   │       │   │   │   ├── c14nPrefixQname.xml
    │   │       │   │   │   ├── c14nPrefixQnameXpathElem.xml
    │   │       │   │   │   ├── c14nPrefix.xml
    │   │       │   │   │   ├── c14nQnameElem.xml
    │   │       │   │   │   ├── c14nQname.xml
    │   │       │   │   │   ├── c14nQnameXpathElem.xml
    │   │       │   │   │   ├── c14nTrim.xml
    │   │       │   │   │   ├── doc.dtd
    │   │       │   │   │   ├── doc.xsl
    │   │       │   │   │   ├── inC14N1.xml
    │   │       │   │   │   ├── inC14N2.xml
    │   │       │   │   │   ├── inC14N3.xml
    │   │       │   │   │   ├── inC14N4.xml
    │   │       │   │   │   ├── inC14N5.xml
    │   │       │   │   │   ├── inC14N6.xml
    │   │       │   │   │   ├── inNsContent.xml
    │   │       │   │   │   ├── inNsDefault.xml
    │   │       │   │   │   ├── inNsPushdown.xml
    │   │       │   │   │   ├── inNsRedecl.xml
    │   │       │   │   │   ├── inNsSort.xml
    │   │       │   │   │   ├── inNsSuperfluous.xml
    │   │       │   │   │   ├── inNsXml.xml
    │   │       │   │   │   ├── out_inC14N1_c14nComment.xml
    │   │       │   │   │   ├── out_inC14N1_c14nDefault.xml
    │   │       │   │   │   ├── out_inC14N2_c14nDefault.xml
    │   │       │   │   │   ├── out_inC14N2_c14nTrim.xml
    │   │       │   │   │   ├── out_inC14N3_c14nDefault.xml
    │   │       │   │   │   ├── out_inC14N3_c14nPrefix.xml
    │   │       │   │   │   ├── out_inC14N3_c14nTrim.xml
    │   │       │   │   │   ├── out_inC14N4_c14nDefault.xml
    │   │       │   │   │   ├── out_inC14N4_c14nTrim.xml
    │   │       │   │   │   ├── out_inC14N5_c14nDefault.xml
    │   │       │   │   │   ├── out_inC14N5_c14nTrim.xml
    │   │       │   │   │   ├── out_inC14N6_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsContent_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsContent_c14nPrefixQnameXpathElem.xml
    │   │       │   │   │   ├── out_inNsContent_c14nQnameElem.xml
    │   │       │   │   │   ├── out_inNsContent_c14nQnameXpathElem.xml
    │   │       │   │   │   ├── out_inNsDefault_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsDefault_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsPushdown_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsPushdown_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsRedecl_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsRedecl_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsSort_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsSort_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsSuperfluous_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsSuperfluous_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsXml_c14nDefault.xml
    │   │       │   │   │   ├── out_inNsXml_c14nPrefixQname.xml
    │   │       │   │   │   ├── out_inNsXml_c14nPrefix.xml
    │   │       │   │   │   ├── out_inNsXml_c14nQname.xml
    │   │       │   │   │   ├── README
    │   │       │   │   │   └── world.txt
    │   │       │   │   ├── expat224_utf8_bug.xml
    │   │       │   │   ├── simple-ns.xml
    │   │       │   │   ├── simple.xml
    │   │       │   │   ├── test.xml
    │   │       │   │   └── test.xml.out
    │   │       │   ├── xmltests.py
    │   │       │   ├── zip_cp437_header.zip
    │   │       │   ├── zipdir.zip
    │   │       │   └── ziptestdata
    │   │       │       ├── exe_with_z64
    │   │       │       ├── exe_with_zip
    │   │       │       ├── header.sh
    │   │       │       ├── __pycache__
    │   │       │       │   ├── testdata_module_inside_zip.cpython-311.opt-1.pyc
    │   │       │       │   ├── testdata_module_inside_zip.cpython-311.opt-2.pyc
    │   │       │       │   └── testdata_module_inside_zip.cpython-311.pyc
    │   │       │       ├── README.md
    │   │       │       └── testdata_module_inside_zip.py
    │   │       ├── textwrap.py
    │   │       ├── this.py
    │   │       ├── _threading_local.py
    │   │       ├── threading.py
    │   │       ├── timeit.py
    │   │       ├── tkinter
    │   │       │   ├── colorchooser.py
    │   │       │   ├── commondialog.py
    │   │       │   ├── constants.py
    │   │       │   ├── dialog.py
    │   │       │   ├── dnd.py
    │   │       │   ├── filedialog.py
    │   │       │   ├── font.py
    │   │       │   ├── __init__.py
    │   │       │   ├── __main__.py
    │   │       │   ├── messagebox.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── colorchooser.cpython-311.opt-1.pyc
    │   │       │   │   ├── colorchooser.cpython-311.opt-2.pyc
    │   │       │   │   ├── colorchooser.cpython-311.pyc
    │   │       │   │   ├── commondialog.cpython-311.opt-1.pyc
    │   │       │   │   ├── commondialog.cpython-311.opt-2.pyc
    │   │       │   │   ├── commondialog.cpython-311.pyc
    │   │       │   │   ├── constants.cpython-311.opt-1.pyc
    │   │       │   │   ├── constants.cpython-311.opt-2.pyc
    │   │       │   │   ├── constants.cpython-311.pyc
    │   │       │   │   ├── dialog.cpython-311.opt-1.pyc
    │   │       │   │   ├── dialog.cpython-311.opt-2.pyc
    │   │       │   │   ├── dialog.cpython-311.pyc
    │   │       │   │   ├── dnd.cpython-311.opt-1.pyc
    │   │       │   │   ├── dnd.cpython-311.opt-2.pyc
    │   │       │   │   ├── dnd.cpython-311.pyc
    │   │       │   │   ├── filedialog.cpython-311.opt-1.pyc
    │   │       │   │   ├── filedialog.cpython-311.opt-2.pyc
    │   │       │   │   ├── filedialog.cpython-311.pyc
    │   │       │   │   ├── font.cpython-311.opt-1.pyc
    │   │       │   │   ├── font.cpython-311.opt-2.pyc
    │   │       │   │   ├── font.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── messagebox.cpython-311.opt-1.pyc
    │   │       │   │   ├── messagebox.cpython-311.opt-2.pyc
    │   │       │   │   ├── messagebox.cpython-311.pyc
    │   │       │   │   ├── scrolledtext.cpython-311.opt-1.pyc
    │   │       │   │   ├── scrolledtext.cpython-311.opt-2.pyc
    │   │       │   │   ├── scrolledtext.cpython-311.pyc
    │   │       │   │   ├── simpledialog.cpython-311.opt-1.pyc
    │   │       │   │   ├── simpledialog.cpython-311.opt-2.pyc
    │   │       │   │   ├── simpledialog.cpython-311.pyc
    │   │       │   │   ├── tix.cpython-311.opt-1.pyc
    │   │       │   │   ├── tix.cpython-311.opt-2.pyc
    │   │       │   │   ├── tix.cpython-311.pyc
    │   │       │   │   ├── ttk.cpython-311.opt-1.pyc
    │   │       │   │   ├── ttk.cpython-311.opt-2.pyc
    │   │       │   │   └── ttk.cpython-311.pyc
    │   │       │   ├── scrolledtext.py
    │   │       │   ├── simpledialog.py
    │   │       │   ├── test
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── support.cpython-311.pyc
    │   │       │   │   │   ├── widget_tests.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── widget_tests.cpython-311.opt-2.pyc
    │   │       │   │   │   └── widget_tests.cpython-311.pyc
    │   │       │   │   ├── README
    │   │       │   │   ├── support.py
    │   │       │   │   ├── test_tkinter
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_colorchooser.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_colorchooser.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_colorchooser.cpython-311.pyc
    │   │       │   │   │   │   ├── test_font.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_font.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_font.cpython-311.pyc
    │   │       │   │   │   │   ├── test_geometry_managers.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_geometry_managers.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_geometry_managers.cpython-311.pyc
    │   │       │   │   │   │   ├── test_images.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_images.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_images.cpython-311.pyc
    │   │       │   │   │   │   ├── test_loadtk.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_loadtk.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_loadtk.cpython-311.pyc
    │   │       │   │   │   │   ├── test_messagebox.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_messagebox.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_messagebox.cpython-311.pyc
    │   │       │   │   │   │   ├── test_misc.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_misc.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_misc.cpython-311.pyc
    │   │       │   │   │   │   ├── test_simpledialog.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_simpledialog.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_simpledialog.cpython-311.pyc
    │   │       │   │   │   │   ├── test_text.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_text.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_text.cpython-311.pyc
    │   │       │   │   │   │   ├── test_variables.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_variables.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_variables.cpython-311.pyc
    │   │       │   │   │   │   ├── test_widgets.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_widgets.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_widgets.cpython-311.pyc
    │   │       │   │   │   ├── test_colorchooser.py
    │   │       │   │   │   ├── test_font.py
    │   │       │   │   │   ├── test_geometry_managers.py
    │   │       │   │   │   ├── test_images.py
    │   │       │   │   │   ├── test_loadtk.py
    │   │       │   │   │   ├── test_messagebox.py
    │   │       │   │   │   ├── test_misc.py
    │   │       │   │   │   ├── test_simpledialog.py
    │   │       │   │   │   ├── test_text.py
    │   │       │   │   │   ├── test_variables.py
    │   │       │   │   │   └── test_widgets.py
    │   │       │   │   ├── test_ttk
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── test_extensions.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_extensions.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_extensions.cpython-311.pyc
    │   │       │   │   │   │   ├── test_style.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_style.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── test_style.cpython-311.pyc
    │   │       │   │   │   │   ├── test_widgets.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── test_widgets.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── test_widgets.cpython-311.pyc
    │   │       │   │   │   ├── test_extensions.py
    │   │       │   │   │   ├── test_style.py
    │   │       │   │   │   └── test_widgets.py
    │   │       │   │   └── widget_tests.py
    │   │       │   ├── tix.py
    │   │       │   └── ttk.py
    │   │       ├── tokenize.py
    │   │       ├── token.py
    │   │       ├── tomllib
    │   │       │   ├── __init__.py
    │   │       │   ├── _parser.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── _parser.cpython-311.opt-1.pyc
    │   │       │   │   ├── _parser.cpython-311.opt-2.pyc
    │   │       │   │   ├── _parser.cpython-311.pyc
    │   │       │   │   ├── _re.cpython-311.opt-1.pyc
    │   │       │   │   ├── _re.cpython-311.opt-2.pyc
    │   │       │   │   ├── _re.cpython-311.pyc
    │   │       │   │   ├── _types.cpython-311.opt-1.pyc
    │   │       │   │   ├── _types.cpython-311.opt-2.pyc
    │   │       │   │   └── _types.cpython-311.pyc
    │   │       │   ├── _re.py
    │   │       │   └── _types.py
    │   │       ├── traceback.py
    │   │       ├── tracemalloc.py
    │   │       ├── trace.py
    │   │       ├── tty.py
    │   │       ├── turtledemo
    │   │       │   ├── bytedesign.py
    │   │       │   ├── chaos.py
    │   │       │   ├── clock.py
    │   │       │   ├── colormixer.py
    │   │       │   ├── forest.py
    │   │       │   ├── fractalcurves.py
    │   │       │   ├── __init__.py
    │   │       │   ├── lindenmayer.py
    │   │       │   ├── __main__.py
    │   │       │   ├── minimal_hanoi.py
    │   │       │   ├── nim.py
    │   │       │   ├── paint.py
    │   │       │   ├── peace.py
    │   │       │   ├── penrose.py
    │   │       │   ├── planet_and_moon.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── bytedesign.cpython-311.opt-1.pyc
    │   │       │   │   ├── bytedesign.cpython-311.opt-2.pyc
    │   │       │   │   ├── bytedesign.cpython-311.pyc
    │   │       │   │   ├── chaos.cpython-311.opt-1.pyc
    │   │       │   │   ├── chaos.cpython-311.opt-2.pyc
    │   │       │   │   ├── chaos.cpython-311.pyc
    │   │       │   │   ├── clock.cpython-311.opt-1.pyc
    │   │       │   │   ├── clock.cpython-311.opt-2.pyc
    │   │       │   │   ├── clock.cpython-311.pyc
    │   │       │   │   ├── colormixer.cpython-311.opt-1.pyc
    │   │       │   │   ├── colormixer.cpython-311.opt-2.pyc
    │   │       │   │   ├── colormixer.cpython-311.pyc
    │   │       │   │   ├── forest.cpython-311.opt-1.pyc
    │   │       │   │   ├── forest.cpython-311.opt-2.pyc
    │   │       │   │   ├── forest.cpython-311.pyc
    │   │       │   │   ├── fractalcurves.cpython-311.opt-1.pyc
    │   │       │   │   ├── fractalcurves.cpython-311.opt-2.pyc
    │   │       │   │   ├── fractalcurves.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── lindenmayer.cpython-311.opt-1.pyc
    │   │       │   │   ├── lindenmayer.cpython-311.opt-2.pyc
    │   │       │   │   ├── lindenmayer.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── minimal_hanoi.cpython-311.opt-1.pyc
    │   │       │   │   ├── minimal_hanoi.cpython-311.opt-2.pyc
    │   │       │   │   ├── minimal_hanoi.cpython-311.pyc
    │   │       │   │   ├── nim.cpython-311.opt-1.pyc
    │   │       │   │   ├── nim.cpython-311.opt-2.pyc
    │   │       │   │   ├── nim.cpython-311.pyc
    │   │       │   │   ├── paint.cpython-311.opt-1.pyc
    │   │       │   │   ├── paint.cpython-311.opt-2.pyc
    │   │       │   │   ├── paint.cpython-311.pyc
    │   │       │   │   ├── peace.cpython-311.opt-1.pyc
    │   │       │   │   ├── peace.cpython-311.opt-2.pyc
    │   │       │   │   ├── peace.cpython-311.pyc
    │   │       │   │   ├── penrose.cpython-311.opt-1.pyc
    │   │       │   │   ├── penrose.cpython-311.opt-2.pyc
    │   │       │   │   ├── penrose.cpython-311.pyc
    │   │       │   │   ├── planet_and_moon.cpython-311.opt-1.pyc
    │   │       │   │   ├── planet_and_moon.cpython-311.opt-2.pyc
    │   │       │   │   ├── planet_and_moon.cpython-311.pyc
    │   │       │   │   ├── rosette.cpython-311.opt-1.pyc
    │   │       │   │   ├── rosette.cpython-311.opt-2.pyc
    │   │       │   │   ├── rosette.cpython-311.pyc
    │   │       │   │   ├── round_dance.cpython-311.opt-1.pyc
    │   │       │   │   ├── round_dance.cpython-311.opt-2.pyc
    │   │       │   │   ├── round_dance.cpython-311.pyc
    │   │       │   │   ├── sorting_animate.cpython-311.opt-1.pyc
    │   │       │   │   ├── sorting_animate.cpython-311.opt-2.pyc
    │   │       │   │   ├── sorting_animate.cpython-311.pyc
    │   │       │   │   ├── tree.cpython-311.opt-1.pyc
    │   │       │   │   ├── tree.cpython-311.opt-2.pyc
    │   │       │   │   ├── tree.cpython-311.pyc
    │   │       │   │   ├── two_canvases.cpython-311.opt-1.pyc
    │   │       │   │   ├── two_canvases.cpython-311.opt-2.pyc
    │   │       │   │   ├── two_canvases.cpython-311.pyc
    │   │       │   │   ├── yinyang.cpython-311.opt-1.pyc
    │   │       │   │   ├── yinyang.cpython-311.opt-2.pyc
    │   │       │   │   └── yinyang.cpython-311.pyc
    │   │       │   ├── rosette.py
    │   │       │   ├── round_dance.py
    │   │       │   ├── sorting_animate.py
    │   │       │   ├── tree.py
    │   │       │   ├── turtle.cfg
    │   │       │   ├── two_canvases.py
    │   │       │   └── yinyang.py
    │   │       ├── turtle.py
    │   │       ├── types.py
    │   │       ├── typing.py
    │   │       ├── unittest
    │   │       │   ├── async_case.py
    │   │       │   ├── case.py
    │   │       │   ├── __init__.py
    │   │       │   ├── loader.py
    │   │       │   ├── _log.py
    │   │       │   ├── __main__.py
    │   │       │   ├── main.py
    │   │       │   ├── mock.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── async_case.cpython-311.opt-1.pyc
    │   │       │   │   ├── async_case.cpython-311.opt-2.pyc
    │   │       │   │   ├── async_case.cpython-311.pyc
    │   │       │   │   ├── case.cpython-311.opt-1.pyc
    │   │       │   │   ├── case.cpython-311.opt-2.pyc
    │   │       │   │   ├── case.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── loader.cpython-311.opt-1.pyc
    │   │       │   │   ├── loader.cpython-311.opt-2.pyc
    │   │       │   │   ├── loader.cpython-311.pyc
    │   │       │   │   ├── _log.cpython-311.opt-1.pyc
    │   │       │   │   ├── _log.cpython-311.opt-2.pyc
    │   │       │   │   ├── _log.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── main.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   ├── main.cpython-311.opt-2.pyc
    │   │       │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   ├── main.cpython-311.pyc
    │   │       │   │   ├── mock.cpython-311.opt-1.pyc
    │   │       │   │   ├── mock.cpython-311.opt-2.pyc
    │   │       │   │   ├── mock.cpython-311.pyc
    │   │       │   │   ├── result.cpython-311.opt-1.pyc
    │   │       │   │   ├── result.cpython-311.opt-2.pyc
    │   │       │   │   ├── result.cpython-311.pyc
    │   │       │   │   ├── runner.cpython-311.opt-1.pyc
    │   │       │   │   ├── runner.cpython-311.opt-2.pyc
    │   │       │   │   ├── runner.cpython-311.pyc
    │   │       │   │   ├── signals.cpython-311.opt-1.pyc
    │   │       │   │   ├── signals.cpython-311.opt-2.pyc
    │   │       │   │   ├── signals.cpython-311.pyc
    │   │       │   │   ├── suite.cpython-311.opt-1.pyc
    │   │       │   │   ├── suite.cpython-311.opt-2.pyc
    │   │       │   │   ├── suite.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   └── util.cpython-311.pyc
    │   │       │   ├── result.py
    │   │       │   ├── runner.py
    │   │       │   ├── signals.py
    │   │       │   ├── suite.py
    │   │       │   ├── test
    │   │       │   │   ├── dummy.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── __main__.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── dummy.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── dummy.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── dummy.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── support.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── support.cpython-311.pyc
    │   │       │   │   │   ├── test_assertions.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_assertions.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_assertions.cpython-311.pyc
    │   │       │   │   │   ├── test_async_case.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_async_case.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_async_case.cpython-311.pyc
    │   │       │   │   │   ├── test_break.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_break.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_break.cpython-311.pyc
    │   │       │   │   │   ├── test_case.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_case.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_case.cpython-311.pyc
    │   │       │   │   │   ├── test_discovery.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_discovery.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_discovery.cpython-311.pyc
    │   │       │   │   │   ├── test_functiontestcase.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_functiontestcase.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_functiontestcase.cpython-311.pyc
    │   │       │   │   │   ├── test_loader.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_loader.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_loader.cpython-311.pyc
    │   │       │   │   │   ├── test_program.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_program.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_program.cpython-311.pyc
    │   │       │   │   │   ├── test_result.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_result.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_result.cpython-311.pyc
    │   │       │   │   │   ├── test_runner.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_runner.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_runner.cpython-311.pyc
    │   │       │   │   │   ├── test_setups.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_setups.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_setups.cpython-311.pyc
    │   │       │   │   │   ├── test_skipping.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_skipping.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_skipping.cpython-311.pyc
    │   │       │   │   │   ├── test_suite.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── test_suite.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── test_suite.cpython-311.pyc
    │   │       │   │   │   ├── _test_warnings.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── _test_warnings.cpython-311.opt-2.pyc
    │   │       │   │   │   └── _test_warnings.cpython-311.pyc
    │   │       │   │   ├── support.py
    │   │       │   │   ├── test_assertions.py
    │   │       │   │   ├── test_async_case.py
    │   │       │   │   ├── test_break.py
    │   │       │   │   ├── test_case.py
    │   │       │   │   ├── test_discovery.py
    │   │       │   │   ├── test_functiontestcase.py
    │   │       │   │   ├── test_loader.py
    │   │       │   │   ├── testmock
    │   │       │   │   │   ├── __init__.py
    │   │       │   │   │   ├── __main__.py
    │   │       │   │   │   ├── __pycache__
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── __main__.cpython-311.pyc
    │   │       │   │   │   │   ├── support.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── support.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── support.cpython-311.pyc
    │   │       │   │   │   │   ├── testasync.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testasync.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testasync.cpython-311.pyc
    │   │       │   │   │   │   ├── testcallable.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testcallable.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testcallable.cpython-311.pyc
    │   │       │   │   │   │   ├── testhelpers.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testhelpers.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testhelpers.cpython-311.pyc
    │   │       │   │   │   │   ├── testmagicmethods.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testmagicmethods.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testmagicmethods.cpython-311.pyc
    │   │       │   │   │   │   ├── testmock.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testmock.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testmock.cpython-311.pyc
    │   │       │   │   │   │   ├── testpatch.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testpatch.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testpatch.cpython-311.pyc
    │   │       │   │   │   │   ├── testsealable.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testsealable.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testsealable.cpython-311.pyc
    │   │       │   │   │   │   ├── testsentinel.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testsentinel.cpython-311.opt-2.pyc
    │   │       │   │   │   │   ├── testsentinel.cpython-311.pyc
    │   │       │   │   │   │   ├── testwith.cpython-311.opt-1.pyc
    │   │       │   │   │   │   ├── testwith.cpython-311.opt-2.pyc
    │   │       │   │   │   │   └── testwith.cpython-311.pyc
    │   │       │   │   │   ├── support.py
    │   │       │   │   │   ├── testasync.py
    │   │       │   │   │   ├── testcallable.py
    │   │       │   │   │   ├── testhelpers.py
    │   │       │   │   │   ├── testmagicmethods.py
    │   │       │   │   │   ├── testmock.py
    │   │       │   │   │   ├── testpatch.py
    │   │       │   │   │   ├── testsealable.py
    │   │       │   │   │   ├── testsentinel.py
    │   │       │   │   │   └── testwith.py
    │   │       │   │   ├── test_program.py
    │   │       │   │   ├── test_result.py
    │   │       │   │   ├── test_runner.py
    │   │       │   │   ├── test_setups.py
    │   │       │   │   ├── test_skipping.py
    │   │       │   │   ├── test_suite.py
    │   │       │   │   └── _test_warnings.py
    │   │       │   └── util.py
    │   │       ├── urllib
    │   │       │   ├── error.py
    │   │       │   ├── __init__.py
    │   │       │   ├── parse.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── error.cpython-311.opt-1.pyc
    │   │       │   │   ├── error.cpython-311.opt-2.pyc
    │   │       │   │   ├── error.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── parse.cpython-311.opt-1.pyc
    │   │       │   │   ├── parse.cpython-311.opt-2.pyc
    │   │       │   │   ├── parse.cpython-311.pyc
    │   │       │   │   ├── request.cpython-311.opt-1.pyc
    │   │       │   │   ├── request.cpython-311.opt-2.pyc
    │   │       │   │   ├── request.cpython-311.pyc
    │   │       │   │   ├── response.cpython-311.opt-1.pyc
    │   │       │   │   ├── response.cpython-311.opt-2.pyc
    │   │       │   │   ├── response.cpython-311.pyc
    │   │       │   │   ├── robotparser.cpython-311.opt-1.pyc
    │   │       │   │   ├── robotparser.cpython-311.opt-2.pyc
    │   │       │   │   └── robotparser.cpython-311.pyc
    │   │       │   ├── request.py
    │   │       │   ├── response.py
    │   │       │   └── robotparser.py
    │   │       ├── uuid.py
    │   │       ├── uu.py
    │   │       ├── venv
    │   │       │   ├── __init__.py
    │   │       │   ├── __main__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __main__.cpython-311.opt-2.pyc
    │   │       │   │   └── __main__.cpython-311.pyc
    │   │       │   └── scripts
    │   │       │       ├── common
    │   │       │       │   ├── activate
    │   │       │       │   └── Activate.ps1
    │   │       │       └── posix
    │   │       │           ├── activate.csh
    │   │       │           └── activate.fish
    │   │       ├── warnings.py
    │   │       ├── wave.py
    │   │       ├── weakref.py
    │   │       ├── _weakrefset.py
    │   │       ├── webbrowser.py
    │   │       ├── wsgiref
    │   │       │   ├── handlers.py
    │   │       │   ├── headers.py
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── handlers.cpython-311.opt-1.pyc
    │   │       │   │   ├── handlers.cpython-311.opt-2.pyc
    │   │       │   │   ├── handlers.cpython-311.pyc
    │   │       │   │   ├── headers.cpython-311.opt-1.pyc
    │   │       │   │   ├── headers.cpython-311.opt-2.pyc
    │   │       │   │   ├── headers.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── simple_server.cpython-311.opt-1.pyc
    │   │       │   │   ├── simple_server.cpython-311.opt-2.pyc
    │   │       │   │   ├── simple_server.cpython-311.pyc
    │   │       │   │   ├── types.cpython-311.opt-1.pyc
    │   │       │   │   ├── types.cpython-311.opt-2.pyc
    │   │       │   │   ├── types.cpython-311.pyc
    │   │       │   │   ├── util.cpython-311.opt-1.pyc
    │   │       │   │   ├── util.cpython-311.opt-2.pyc
    │   │       │   │   ├── util.cpython-311.pyc
    │   │       │   │   ├── validate.cpython-311.opt-1.pyc
    │   │       │   │   ├── validate.cpython-311.opt-2.pyc
    │   │       │   │   └── validate.cpython-311.pyc
    │   │       │   ├── simple_server.py
    │   │       │   ├── types.py
    │   │       │   ├── util.py
    │   │       │   └── validate.py
    │   │       ├── xdrlib.py
    │   │       ├── xml
    │   │       │   ├── dom
    │   │       │   │   ├── domreg.py
    │   │       │   │   ├── expatbuilder.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   ├── minicompat.py
    │   │       │   │   ├── minidom.py
    │   │       │   │   ├── NodeFilter.py
    │   │       │   │   ├── pulldom.py
    │   │       │   │   ├── __pycache__
    │   │       │   │   │   ├── domreg.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── domreg.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── domreg.cpython-311.pyc
    │   │       │   │   │   ├── expatbuilder.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── expatbuilder.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── expatbuilder.cpython-311.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   │   ├── minicompat.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── minicompat.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── minicompat.cpython-311.pyc
    │   │       │   │   │   ├── minidom.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── minidom.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── minidom.cpython-311.pyc
    │   │       │   │   │   ├── NodeFilter.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── NodeFilter.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── NodeFilter.cpython-311.pyc
    │   │       │   │   │   ├── pulldom.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── pulldom.cpython-311.opt-2.pyc
    │   │       │   │   │   ├── pulldom.cpython-311.pyc
    │   │       │   │   │   ├── xmlbuilder.cpython-311.opt-1.pyc
    │   │       │   │   │   ├── xmlbuilder.cpython-311.opt-2.pyc
    │   │       │   │   │   └── xmlbuilder.cpython-311.pyc
    │   │       │   │   └── xmlbuilder.py
    │   │       │   ├── etree
    │   │       │   │   ├── cElementTree.py
    │   │       │   │   ├── ElementInclude.py
    │   │       │   │   ├── ElementPath.py
    │   │       │   │   ├── ElementTree.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── cElementTree.cpython-311.opt-1.pyc
    │   │       │   │       ├── cElementTree.cpython-311.opt-2.pyc
    │   │       │   │       ├── cElementTree.cpython-311.pyc
    │   │       │   │       ├── ElementInclude.cpython-311.opt-1.pyc
    │   │       │   │       ├── ElementInclude.cpython-311.opt-2.pyc
    │   │       │   │       ├── ElementInclude.cpython-311.pyc
    │   │       │   │       ├── ElementPath.cpython-311.opt-1.pyc
    │   │       │   │       ├── ElementPath.cpython-311.opt-2.pyc
    │   │       │   │       ├── ElementPath.cpython-311.pyc
    │   │       │   │       ├── ElementTree.cpython-311.opt-1.pyc
    │   │       │   │       ├── ElementTree.cpython-311.opt-2.pyc
    │   │       │   │       ├── ElementTree.cpython-311.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   ├── __init__.py
    │   │       │   ├── parsers
    │   │       │   │   ├── expat.py
    │   │       │   │   ├── __init__.py
    │   │       │   │   └── __pycache__
    │   │       │   │       ├── expat.cpython-311.opt-1.pyc
    │   │       │   │       ├── expat.cpython-311.opt-2.pyc
    │   │       │   │       ├── expat.cpython-311.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │       ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │       └── __init__.cpython-311.pyc
    │   │       │   ├── __pycache__
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   └── __init__.cpython-311.pyc
    │   │       │   └── sax
    │   │       │       ├── _exceptions.py
    │   │       │       ├── expatreader.py
    │   │       │       ├── handler.py
    │   │       │       ├── __init__.py
    │   │       │       ├── __pycache__
    │   │       │       │   ├── _exceptions.cpython-311.opt-1.pyc
    │   │       │       │   ├── _exceptions.cpython-311.opt-2.pyc
    │   │       │       │   ├── _exceptions.cpython-311.pyc
    │   │       │       │   ├── expatreader.cpython-311.opt-1.pyc
    │   │       │       │   ├── expatreader.cpython-311.opt-2.pyc
    │   │       │       │   ├── expatreader.cpython-311.pyc
    │   │       │       │   ├── handler.cpython-311.opt-1.pyc
    │   │       │       │   ├── handler.cpython-311.opt-2.pyc
    │   │       │       │   ├── handler.cpython-311.pyc
    │   │       │       │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │       │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │       │   ├── __init__.cpython-311.pyc
    │   │       │       │   ├── saxutils.cpython-311.opt-1.pyc
    │   │       │       │   ├── saxutils.cpython-311.opt-2.pyc
    │   │       │       │   ├── saxutils.cpython-311.pyc
    │   │       │       │   ├── xmlreader.cpython-311.opt-1.pyc
    │   │       │       │   ├── xmlreader.cpython-311.opt-2.pyc
    │   │       │       │   └── xmlreader.cpython-311.pyc
    │   │       │       ├── saxutils.py
    │   │       │       └── xmlreader.py
    │   │       ├── xmlrpc
    │   │       │   ├── client.py
    │   │       │   ├── __init__.py
    │   │       │   ├── __pycache__
    │   │       │   │   ├── client.cpython-311.opt-1.pyc
    │   │       │   │   ├── client.cpython-311.opt-2.pyc
    │   │       │   │   ├── client.cpython-311.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-1.pyc
    │   │       │   │   ├── __init__.cpython-311.opt-2.pyc
    │   │       │   │   ├── __init__.cpython-311.pyc
    │   │       │   │   ├── server.cpython-311.opt-1.pyc
    │   │       │   │   ├── server.cpython-311.opt-2.pyc
    │   │       │   │   └── server.cpython-311.pyc
    │   │       │   └── server.py
    │   │       ├── zipapp.py
    │   │       ├── zipfile.py
    │   │       ├── zipimport.py
    │   │       └── zoneinfo
    │   │           ├── _common.py
    │   │           ├── __init__.py
    │   │           ├── __pycache__
    │   │           │   ├── _common.cpython-311.opt-1.pyc
    │   │           │   ├── _common.cpython-311.opt-2.pyc
    │   │           │   ├── _common.cpython-311.pyc
    │   │           │   ├── __init__.cpython-311.opt-1.pyc
    │   │           │   ├── __init__.cpython-311.opt-2.pyc
    │   │           │   ├── __init__.cpython-311.pyc
    │   │           │   ├── _tzpath.cpython-311.opt-1.pyc
    │   │           │   ├── _tzpath.cpython-311.opt-2.pyc
    │   │           │   ├── _tzpath.cpython-311.pyc
    │   │           │   ├── _zoneinfo.cpython-311.opt-1.pyc
    │   │           │   ├── _zoneinfo.cpython-311.opt-2.pyc
    │   │           │   └── _zoneinfo.cpython-311.pyc
    │   │           ├── _tzpath.py
    │   │           └── _zoneinfo.py
    │   └── share
    │       └── man
    │           └── man1
    │               ├── python3.1 -> python3.11.1
    │               └── python3.11.1
    └── share
        ├── fonts
        │   └── truetype
        │       └── dejavu
        │           ├── DejaVuSans-Bold.ttf
        │           ├── DejaVuSansMono-Bold.ttf
        │           ├── DejaVuSansMono.ttf
        │           ├── DejaVuSans.ttf
        │           ├── DejaVuSerif-Bold.ttf
        │           └── DejaVuSerif.ttf
        ├── tcltk
        │   ├── tcl8.6
        │   │   ├── auto.tcl
        │   │   ├── clock.tcl
        │   │   ├── encoding
        │   │   │   ├── ascii.enc
        │   │   │   ├── big5.enc
        │   │   │   ├── cp1250.enc
        │   │   │   ├── cp1251.enc
        │   │   │   ├── cp1252.enc
        │   │   │   ├── cp1253.enc
        │   │   │   ├── cp1254.enc
        │   │   │   ├── cp1255.enc
        │   │   │   ├── cp1256.enc
        │   │   │   ├── cp1257.enc
        │   │   │   ├── cp1258.enc
        │   │   │   ├── cp437.enc
        │   │   │   ├── cp737.enc
        │   │   │   ├── cp775.enc
        │   │   │   ├── cp850.enc
        │   │   │   ├── cp852.enc
        │   │   │   ├── cp855.enc
        │   │   │   ├── cp857.enc
        │   │   │   ├── cp860.enc
        │   │   │   ├── cp861.enc
        │   │   │   ├── cp862.enc
        │   │   │   ├── cp863.enc
        │   │   │   ├── cp864.enc
        │   │   │   ├── cp865.enc
        │   │   │   ├── cp866.enc
        │   │   │   ├── cp869.enc
        │   │   │   ├── cp874.enc
        │   │   │   ├── cp932.enc
        │   │   │   ├── cp936.enc
        │   │   │   ├── cp949.enc
        │   │   │   ├── cp950.enc
        │   │   │   ├── dingbats.enc
        │   │   │   ├── ebcdic.enc
        │   │   │   ├── euc-cn.enc
        │   │   │   ├── euc-jp.enc
        │   │   │   ├── euc-kr.enc
        │   │   │   ├── gb12345.enc
        │   │   │   ├── gb1988.enc
        │   │   │   ├── gb2312.enc
        │   │   │   ├── gb2312-raw.enc
        │   │   │   ├── iso2022.enc
        │   │   │   ├── iso2022-jp.enc
        │   │   │   ├── iso2022-kr.enc
        │   │   │   ├── iso8859-10.enc
        │   │   │   ├── iso8859-13.enc
        │   │   │   ├── iso8859-14.enc
        │   │   │   ├── iso8859-15.enc
        │   │   │   ├── iso8859-16.enc
        │   │   │   ├── iso8859-1.enc
        │   │   │   ├── iso8859-2.enc
        │   │   │   ├── iso8859-3.enc
        │   │   │   ├── iso8859-4.enc
        │   │   │   ├── iso8859-5.enc
        │   │   │   ├── iso8859-6.enc
        │   │   │   ├── iso8859-7.enc
        │   │   │   ├── iso8859-8.enc
        │   │   │   ├── iso8859-9.enc
        │   │   │   ├── jis0201.enc
        │   │   │   ├── jis0208.enc
        │   │   │   ├── jis0212.enc
        │   │   │   ├── koi8-r.enc
        │   │   │   ├── koi8-u.enc
        │   │   │   ├── ksc5601.enc
        │   │   │   ├── macCentEuro.enc
        │   │   │   ├── macCroatian.enc
        │   │   │   ├── macCyrillic.enc
        │   │   │   ├── macDingbats.enc
        │   │   │   ├── macGreek.enc
        │   │   │   ├── macIceland.enc
        │   │   │   ├── macJapan.enc
        │   │   │   ├── macRoman.enc
        │   │   │   ├── macRomania.enc
        │   │   │   ├── macThai.enc
        │   │   │   ├── macTurkish.enc
        │   │   │   ├── macUkraine.enc
        │   │   │   ├── shiftjis.enc
        │   │   │   ├── symbol.enc
        │   │   │   └── tis-620.enc
        │   │   ├── history.tcl
        │   │   ├── http1.0
        │   │   │   ├── http.tcl
        │   │   │   └── pkgIndex.tcl
        │   │   ├── init.tcl
        │   │   ├── msgs
        │   │   │   ├── af.msg
        │   │   │   ├── af_za.msg
        │   │   │   ├── ar_in.msg
        │   │   │   ├── ar_jo.msg
        │   │   │   ├── ar_lb.msg
        │   │   │   ├── ar.msg
        │   │   │   ├── ar_sy.msg
        │   │   │   ├── be.msg
        │   │   │   ├── bg.msg
        │   │   │   ├── bn_in.msg
        │   │   │   ├── bn.msg
        │   │   │   ├── ca.msg
        │   │   │   ├── cs.msg
        │   │   │   ├── da.msg
        │   │   │   ├── de_at.msg
        │   │   │   ├── de_be.msg
        │   │   │   ├── de.msg
        │   │   │   ├── el.msg
        │   │   │   ├── en_au.msg
        │   │   │   ├── en_be.msg
        │   │   │   ├── en_bw.msg
        │   │   │   ├── en_ca.msg
        │   │   │   ├── en_gb.msg
        │   │   │   ├── en_hk.msg
        │   │   │   ├── en_ie.msg
        │   │   │   ├── en_in.msg
        │   │   │   ├── en_nz.msg
        │   │   │   ├── en_ph.msg
        │   │   │   ├── en_sg.msg
        │   │   │   ├── en_za.msg
        │   │   │   ├── en_zw.msg
        │   │   │   ├── eo.msg
        │   │   │   ├── es_ar.msg
        │   │   │   ├── es_bo.msg
        │   │   │   ├── es_cl.msg
        │   │   │   ├── es_co.msg
        │   │   │   ├── es_cr.msg
        │   │   │   ├── es_do.msg
        │   │   │   ├── es_ec.msg
        │   │   │   ├── es_gt.msg
        │   │   │   ├── es_hn.msg
        │   │   │   ├── es.msg
        │   │   │   ├── es_mx.msg
        │   │   │   ├── es_ni.msg
        │   │   │   ├── es_pa.msg
        │   │   │   ├── es_pe.msg
        │   │   │   ├── es_pr.msg
        │   │   │   ├── es_py.msg
        │   │   │   ├── es_sv.msg
        │   │   │   ├── es_uy.msg
        │   │   │   ├── es_ve.msg
        │   │   │   ├── et.msg
        │   │   │   ├── eu_es.msg
        │   │   │   ├── eu.msg
        │   │   │   ├── fa_in.msg
        │   │   │   ├── fa_ir.msg
        │   │   │   ├── fa.msg
        │   │   │   ├── fi.msg
        │   │   │   ├── fo_fo.msg
        │   │   │   ├── fo.msg
        │   │   │   ├── fr_be.msg
        │   │   │   ├── fr_ca.msg
        │   │   │   ├── fr_ch.msg
        │   │   │   ├── fr.msg
        │   │   │   ├── ga_ie.msg
        │   │   │   ├── ga.msg
        │   │   │   ├── gl_es.msg
        │   │   │   ├── gl.msg
        │   │   │   ├── gv_gb.msg
        │   │   │   ├── gv.msg
        │   │   │   ├── he.msg
        │   │   │   ├── hi_in.msg
        │   │   │   ├── hi.msg
        │   │   │   ├── hr.msg
        │   │   │   ├── hu.msg
        │   │   │   ├── id_id.msg
        │   │   │   ├── id.msg
        │   │   │   ├── is.msg
        │   │   │   ├── it_ch.msg
        │   │   │   ├── it.msg
        │   │   │   ├── ja.msg
        │   │   │   ├── kl_gl.msg
        │   │   │   ├── kl.msg
        │   │   │   ├── kok_in.msg
        │   │   │   ├── kok.msg
        │   │   │   ├── ko_kr.msg
        │   │   │   ├── ko.msg
        │   │   │   ├── kw_gb.msg
        │   │   │   ├── kw.msg
        │   │   │   ├── lt.msg
        │   │   │   ├── lv.msg
        │   │   │   ├── mk.msg
        │   │   │   ├── mr_in.msg
        │   │   │   ├── mr.msg
        │   │   │   ├── ms.msg
        │   │   │   ├── ms_my.msg
        │   │   │   ├── mt.msg
        │   │   │   ├── nb.msg
        │   │   │   ├── nl_be.msg
        │   │   │   ├── nl.msg
        │   │   │   ├── nn.msg
        │   │   │   ├── pl.msg
        │   │   │   ├── pt_br.msg
        │   │   │   ├── pt.msg
        │   │   │   ├── ro.msg
        │   │   │   ├── ru.msg
        │   │   │   ├── ru_ua.msg
        │   │   │   ├── sh.msg
        │   │   │   ├── sk.msg
        │   │   │   ├── sl.msg
        │   │   │   ├── sq.msg
        │   │   │   ├── sr.msg
        │   │   │   ├── sv.msg
        │   │   │   ├── sw.msg
        │   │   │   ├── ta_in.msg
        │   │   │   ├── ta.msg
        │   │   │   ├── te_in.msg
        │   │   │   ├── te.msg
        │   │   │   ├── th.msg
        │   │   │   ├── tr.msg
        │   │   │   ├── uk.msg
        │   │   │   ├── vi.msg
        │   │   │   ├── zh_cn.msg
        │   │   │   ├── zh_hk.msg
        │   │   │   ├── zh.msg
        │   │   │   ├── zh_sg.msg
        │   │   │   └── zh_tw.msg
        │   │   ├── opt0.4
        │   │   │   ├── optparse.tcl
        │   │   │   └── pkgIndex.tcl
        │   │   ├── package.tcl
        │   │   ├── parray.tcl
        │   │   ├── safe.tcl
        │   │   ├── tcl8
        │   │   │   ├── http-2.9.1.tm
        │   │   │   ├── msgcat-1.6.1.tm
        │   │   │   ├── platform
        │   │   │   │   └── shell-1.1.4.tm
        │   │   │   ├── platform-1.0.14.tm
        │   │   │   └── tcltest-2.5.1.tm
        │   │   ├── tclAppInit.c
        │   │   ├── tclIndex
        │   │   ├── tm.tcl
        │   │   └── word.tcl
        │   └── tk8.6
        │       ├── bgerror.tcl
        │       ├── button.tcl
        │       ├── choosedir.tcl
        │       ├── clrpick.tcl
        │       ├── comdlg.tcl
        │       ├── console.tcl
        │       ├── dialog.tcl
        │       ├── entry.tcl
        │       ├── focus.tcl
        │       ├── fontchooser.tcl
        │       ├── iconlist.tcl
        │       ├── icons.tcl
        │       ├── images
        │       │   ├── logo100.gif
        │       │   ├── logo64.gif
        │       │   ├── logo.eps
        │       │   ├── logoLarge.gif
        │       │   ├── logoMed.gif
        │       │   ├── pwrdLogo100.gif
        │       │   ├── pwrdLogo150.gif
        │       │   ├── pwrdLogo175.gif
        │       │   ├── pwrdLogo200.gif
        │       │   ├── pwrdLogo75.gif
        │       │   ├── pwrdLogo.eps
        │       │   ├── README
        │       │   └── tai-ku.gif
        │       ├── listbox.tcl
        │       ├── megawidget.tcl
        │       ├── menu.tcl
        │       ├── mkpsenc.tcl
        │       ├── msgbox.tcl
        │       ├── msgs
        │       │   ├── cs.msg
        │       │   ├── da.msg
        │       │   ├── de.msg
        │       │   ├── el.msg
        │       │   ├── en_gb.msg
        │       │   ├── en.msg
        │       │   ├── eo.msg
        │       │   ├── es.msg
        │       │   ├── fr.msg
        │       │   ├── hu.msg
        │       │   ├── it.msg
        │       │   ├── nl.msg
        │       │   ├── pl.msg
        │       │   ├── pt.msg
        │       │   ├── ru.msg
        │       │   └── sv.msg
        │       ├── obsolete.tcl
        │       ├── optMenu.tcl
        │       ├── palette.tcl
        │       ├── panedwindow.tcl
        │       ├── safetk.tcl
        │       ├── scale.tcl
        │       ├── scrlbar.tcl
        │       ├── spinbox.tcl
        │       ├── tclIndex
        │       ├── tearoff.tcl
        │       ├── text.tcl
        │       ├── tkAppInit.c
        │       ├── tkfbox.tcl
        │       ├── tk.tcl
        │       ├── ttk
        │       │   ├── altTheme.tcl
        │       │   ├── aquaTheme.tcl
        │       │   ├── button.tcl
        │       │   ├── clamTheme.tcl
        │       │   ├── classicTheme.tcl
        │       │   ├── combobox.tcl
        │       │   ├── cursors.tcl
        │       │   ├── defaults.tcl
        │       │   ├── entry.tcl
        │       │   ├── fonts.tcl
        │       │   ├── menubutton.tcl
        │       │   ├── notebook.tcl
        │       │   ├── panedwindow.tcl
        │       │   ├── progress.tcl
        │       │   ├── scale.tcl
        │       │   ├── scrollbar.tcl
        │       │   ├── sizegrip.tcl
        │       │   ├── spinbox.tcl
        │       │   ├── treeview.tcl
        │       │   ├── ttk.tcl
        │       │   ├── utils.tcl
        │       │   ├── vistaTheme.tcl
        │       │   ├── winTheme.tcl
        │       │   └── xpTheme.tcl
        │       ├── unsupported.tcl
        │       └── xmfbox.tcl
        └── xml
            └── fontconfig
                └── fonts.dtd
```
