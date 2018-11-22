Build Instructions
==================

Compile example files with the following gcc flags:
```
gcc -o bot bot.c `pkg-config --cflags --libs libstrophe` -lmosquitto -lpthread
```

Run example files with the following commands:
- Alda: `LD_LIBRARY_PATH=/usr/local/lib/:$LD_LIBRARY_PATH ./bot alda@ci40.xmpp.carlos.com masteriot`
- Carlos: `LD_LIBRARY_PATH=/usr/lib/:$LD_LIBRARY_PATH ./bot bot@ci40.xmpp.carlos.com masteriot`