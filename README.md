# version 1.1	initial version

Copyright (c) 2017 Paul van Haastrecht <paulvha@hotmail.com>

This PPD42 utility willread, display and log the data from a 
PPD42NJ (GROOVE) sensor AND (optional) a DYLOS device on Linux.

It has been tested on a Raspberry Pi-3 (Jessie) and with a DC1700.

PPD42 monitor is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by the
Free Software Foundation, either version 3 of the License, or (at your option) any later version.

For detailed documentation about the project see the ppd42monitor.odt
 
Software installation

BCM2835 library installation
Install latest from BCM2835 from : http://www.airspayce.com/mikem/bcm2835/

1. wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.50.tar.gz
2. tar -zxf bcm2835-1.50.tar.gz		// 1.50 = version at current time 
3. cd bcm2835-1.50
4. ./configure
5. sudo make check
6. sudo make install

PPD42 software installation

1. tar -zxf ppd42-1.1.tar.gz	
2. cd ppd42
3. compile to handle PPD42 only :  “./setup.sh  ppd42”
4. compile including Dylos support : “./setup.sh +DYLOS”
5. start ./ppd42 -h for help options
