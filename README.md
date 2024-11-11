# ubi8-python39


## build

```
$ docker build ./ -t python39
$ docker save python39 > ubi8-python39.tar
$ split -b 50M -d ubi8-python39.tar ubi8-python39.tar_ 
```

## load

```
$ cat ubi8-python39.tar_* > ubi8-python39.tar
$ docker load < ubi8-python39.tar
```

