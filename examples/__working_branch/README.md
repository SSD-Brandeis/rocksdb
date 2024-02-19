## Steps to build `rocksdb`:
1. Install a recent toolchain if you're on a older distro. C++17 required (GCC >= 7, Clang >= 5)
2. Go to `rocksdb` directory.
3. ```make static_lib``` (Alternatively, you can also use -j flag)

## Steps to build `working_version`:
1. Build the `rocksdb` first.
2. Go to `rocksdb/examples/__working_version`
3. ```make working_version```

## Steps to generate workload.txt
1. Go to `rocksdb/examples/K-V-Workload-Generator`
2. make `load_gen`
3. ```./load_gen``` [pass the required arguments]
4. ```./move_workload.sh``` (Provide executable permission; if required)

You are all set to run `./working_version`