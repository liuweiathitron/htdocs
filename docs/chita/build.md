
# Build

### Clone chita project

```
git clone git@gitlab.hitron.com:HT-US2/chita.git -b develop_R7.2.4.5_MR_RC23
```

### build sip

```
source setup.sh sip (bitbake arm)
```

### build ims

```
source setup.sh ims (bitbake arm)
```

### combine sip and ims

```
source setup.sh arm
```

### build atom

```
source setup.sh atom (bitbake atom)
```

### combine arm and atom

```
source setup.sh sign
```


