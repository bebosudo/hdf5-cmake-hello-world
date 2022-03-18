# hdf5-cmake-hello-world

A simple HDF5 "Hello world" application to test cmake

Make sure to `module load cmake` and `module load hdf5` or somehow make hdf5 visible to cmake.

```bash
wget https://github.com/bebosudo/hdf5-cmake-hello-world/archive/refs/tags/v0.1.tar.gz
tar -xf v0.1.tar.gz
cd hdf5-cmake-hello-world-0.1/
cmake .
make
```

If everything went ok, the following diff shouldn't return anything:
```console
$ diff <(./myprog) <(echo -n "1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 ")
$
```

Inspired by https://www.scivision.dev/hdf5-with-cmake/
