# nturt_ros

## Introduction

ROS metapackage(package that contains no source for managing other packages) for nturt. It helps to clone all packages used on rpi all at once, and every version only contains stable packages.

## Usage

Clone this package and all submodules(other packages managed by this metapackage) in it by

```bash=
git clone https://github.com/NTURacingTeam/nturt_ros.git --recurse-submodules
```

in the ros workspace source directory(such as ~/ws/src/).

After pulling the update version of this package, update the submodule by

```bash=
git submodule update
```

## Known issue

Since the source and header files for ros msg/srv in `nturt_ros_interface` is generated during compile time, sometimes cmake will run into errors that says it can not find some include files for ros msg/srv. In such case, the easist solution might just be to compile(running `catkin_make`) multiple times until it compiles successfully.
