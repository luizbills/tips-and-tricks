# Get hardware info

## Windows

- motherboard

```
wmic baseboard get Manufacturer,version,serialnumber
```

## Linux

- motherboard

```
sudo cat /sys/devices/virtual/dmi/id/board_{vendor,version,serial}
```
