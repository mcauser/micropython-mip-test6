# MicroPython MIP test 6

One in a series of example repos to test various mpremote mip installation patterns.

#### Install

```
$ mpremote mip install github:mcauser/micropython-mip-test6

Install github:mcauser/micropython-mip-test6
Installing github:mcauser/micropython-mip-test6/package.json to /lib
Installing: /lib/test6a.py
Installing: /lib//test6b.py
Installing: /lib/./test6c.py
Installing: /lib/lib/test6d.py
Installing: /lib//lib/test6e.py
Installing: /lib/../test6f.py
Installing: /lib/foo/test6g.py
Installing: /lib/foo/bar/test6h.py
Installing: /lib/../pow/zap/test6i.py
Done
```

GitHub     | Device
:----------|:-------------
/test6a.py | /lib/test6a.py
/test6b.py | /lib/test6b.py
/test6c.py | /lib/test6c.py
/test6d.py | /lib/lib/test6d.py
/test6e.py | /lib/lib/test6e.py
/test6f.py | /test6f.py
/test6g.py | /lib/foo/test6g.py
/test6h.py | /lib/foo/bar/test6h.py
/test6i.py | /pow/zap/test6i.py

```
$ mpremote repl

>>> import test6a
test6a
>>> import test6b
test6b
>>> import test6c
test6c
>>> import lib.lib.test6d
test6d
>>> import lib.lib.test6e
test6e
>>> import test6f
test6f
>>> import lib.foo.test6g
test6g
>>> import pow.zap.test6i
test6i
```
