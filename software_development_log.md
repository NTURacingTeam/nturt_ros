# National Taiwan University Racing Team Software Development Log
###### tags: `development_log` `NTURT`
##### Group: electrical system group
##### Person in charge: 羅紀翔
##### Authors: 羅紀翔
##### Subsystem: RPI
##### Subsystem number: RPI
##### Software name: ros_metapackage
##### Repository: [github](https://github.com/NTURacingTeam/nturt_ros)
##### Started designing date: 2022/10/6
##### Current version: 1.0
##### Last modified date: 2022/10/13

---

## Engineering goal:

A metapackage for manging other packages used on rpi and easier to clone all packages running all at once.

## Program structure:

Only the source code of `nturt_ros` metapackage is stored in this repository, all source code of other packages is stored in other git repositories and inclueded here using `git submodule`.

## Included libraries:

- 

## Testing environment:

- git 2.25.1

##### Testing hardware:

- asus tuf gaming a15 FA506II-0031A 4800H

##### Operating system:

- ubuntu 20.04

##### Compiler(intepreter) version:

N/A

---

## Testing result of 1.O:

### Cloning this repository with all submodules

running

```bash=
git clone https://github.com/NTURacingTeam/nturt_ros.git --recurse-submodules
```

All submodules cloned successfully.

### Update all submodules after cloning to new version

running

```bash=
git submodule update
```

All submodules updated successfully.

## Todos in 1.O:
