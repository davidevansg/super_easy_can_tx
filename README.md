# super_easy_can_tx
A super easy C implementation of sending CAN messages using SocketCAN C API

## Prerequisites for building 
### Build-essential
```
    $ sudo apt-get update
    $ sudo apt-get install build-essential
```

### CAN-utils
```
    $ sudo apt-get update
    $ sudo apt-get install can-utils
```

### Setup Virtual CAN interface (vcan0)
```
    $ ./scripts/enable_vcan.sh
```

## Build
```
    $ make
```

## Run
```
    $ ./super_easy_tx_can
```
## View
```
    (Terminal 1) - $ candump vcan0
    (Terminal 2) - $ ./super_easy_tx_can
```
