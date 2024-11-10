# ubi8-python39-latest


## build

```
$ docker build ./ -t python39
$ docker save python39 > ubi8-python39-latest.tar
$ split -b 50M -d ubi8-python39-latest.tar ubi8-python39-latest.tar_ 
```

## load

```
$ docker load < ubi8-python39-latest.tar
```

