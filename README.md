# Kyber

A bash script to program kyber crystals


## Setup

  Before using this script, you must have:
  1. Proxmark3 RFID hardware
  2. CLI installed

### OSX

```bash
brew tap proxmark/proxmark3 
brew install proxmark3
```

### Usage

unplug device  
```
ls /dev/cu*
```
plugin device  
```
ls /dev/cu*
```

```
proxmark3 /dev/cu.usbmodem14313301
```

```
lf search 
lf em 4x05dump 0
```

#### Fix locked crystal

Credit to [Ruthsarian](https://www.youtube.com/watch?v=fy56C4CGaBg)

```
lf em 4x05writeword 4
```