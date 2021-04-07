# FreeBSD Specialities

- First, install `devel/gmake` and `ftp/curl`.

- You need to use `CC=clang` even if `cc` is `clang`, e.g.,

```
	gmake CC=clang
```

- To build and run regression tests, you also need to specify gcov path and
make utility, e.g.,

```
	cd tests && \
	env CC=clang GCOV=/usr/bin/gcov MAKE=gmake sh test_exec.sh
```
