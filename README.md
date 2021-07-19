#!/bin/bash
POOL=ethash.unmineable.com:3333
WALLET=TRX:TVLbd2BxymdDpKq2VfCHSH2nCE1PiqRGP7
WORKEER=$(echo $(shuf -i 1000-9999 -n 1)-USER1#5rah-iur7)


./tuyulgpu --algo ETHASH --pool $POOL --user $WALLET.$WORKEER --ethstratum ETHPROXY
