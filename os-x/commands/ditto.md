# ditto




Copy directory hierarchies, create and extract archives.


## Options

  * `-V` - Print a line of output to stderr for every file, symbolic link, and device copied.
  * `--noacl` - Do not preserve ACLs.


## Examples

#### Data migration

```
ditto -V --noacl <source> <destination>
```

