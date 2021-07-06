# Release

### Clone chita project

```
git clone git@gitlab.hitron.com:HT-US2/chita.git -b develop_R7.2.4.5_MR_RC23
```

### build lastes

```
export HTX_TARGET=coda
source setup.sh build
```

### build specific

```
git checkout topic/release/7.2.4.5.1b2
export HTX_TARGET=coda
source setup.sh release
```


