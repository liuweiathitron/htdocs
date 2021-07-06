## Change MAC address

### Backup old data (atom shell)

```
cp -rvf /nvram/itstore /nvram/itstore_backup
```

### Clear old data (atom shell)

```
chattr -R -i /nvram/itstore
rm -rf /nvram/itstore
```

### Prepare new data (arm shell)

according to label and mac rule

```
echo '[macAddr]' > /var/tmp/temp.ini
echo 'ecm=74:9B:E8:42:E6:E0' >> /var/tmp/temp.ini
echo 'emta=74:9B:E8:42:E6:E1' >> /var/tmp/temp.ini
echo 'cmdiag=74:9B:E8:42:E6:E2' >> /var/tmp/temp.ini
echo 'erouter0=74:9B:E8:42:E6:E3' >> /var/tmp/temp.ini
echo 'moca=00:00:00:77:E6:E0' >> /var/tmp/temp.ini
```

### Store new data to itstore (arm cli)

system&gt;ProductionSystem

```
createAsset /var/tmp/temp.ini production.ini 1
```

