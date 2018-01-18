# Mac OS console daemons

## Dependencies
- macOS High Sierra 10.13.x (not tested on older versions)
- libboost1.58

### Using homebrew
```
brew install boost
```

## How to run node daemon
```
./niobiod
```

## How to run simplewallet
Wait for blockchain sync. You should see on node output:
```
2018-Jan-18 11:09:55.621398 INFO    [177.96.42.29:8313 OUT] SYNCHRONIZED OK
2018-Jan-18 11:09:55.621552 INFO    
2018-Jan-18 11:09:55.621552 INFO    **********************************************************************
2018-Jan-18 11:09:55.621552 INFO    You are now synchronized with the network. You may now start simplewallet.
2018-Jan-18 11:09:55.621552 INFO    
2018-Jan-18 11:09:55.621552 INFO    Please note, that the blockchain will be saved only after you quit the daemon with "exit" command or if you use "save" command.
2018-Jan-18 11:09:55.621552 INFO    Otherwise, you will possibly need to synchronize the blockchain again.
2018-Jan-18 11:09:55.621552 INFO    
2018-Jan-18 11:09:55.621552 INFO    Use "help" command to see the list of available commands.
2018-Jan-18 11:09:55.621552 INFO    **********************************************************************
```

After node is synchronized:
```
./simplewallet
```

## How to run miner
```
./miner --address <your-wallet-address>
```