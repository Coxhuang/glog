# Trunk glog

```shell
cmake -DCMAKE_INSTALL_PREFIX=/opt/trunk -DBUILD_SHARED_LIBS=ON ..
make package -j4
```

> 推荐使用 `pkg_check_modules`

```shell
pkg_check_modules(Glog REQUIRED libglog)
message(${Glog_INCLUDE_DIRS})
message(${Glog_LIBRARY_DIRS})
message(${Glog_LIBRARIES})
```

```shell
find_package(glog REQUIRED)
message(${Glog_INCLUDE_DIRS})
message(${Glog_LIBRARY_DIRS})
message(${Glog_LIBRARIES})
```

