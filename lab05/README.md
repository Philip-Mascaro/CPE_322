download and install Mosquitto

```
$ sudo pip3 install -U paho-mqtt
$ git clone https://github.com/eclipse/paho.mqtt.python.git
$ cd ~/iot/lesson5
$ python3 client.py
```
![l5s01.png](images/l5s01.png)
![l5s02.png](images/l5s02.png)

use two terminals, one for each command
```
$ python3 sub.py
$ python3 pub.py
```
![l5s03.png](images/l5s03.png)
![l5s04.png](images/l5s04.png)

at this point I thought it wasn't working because I downloaded Mosquitto on Windows but downloaded Paho on Ubuntu, so I redid the above steps in Windows
![l5s05.png](images/l5s05.png)
![l5s06.png](images/l5s06.png)

at this point I realized that I only needed to run subcpu.py and pubcpu.py

use two terminals, one for each command
```
$ python3 subcpu.py
$ python3 pubcpu.py
```
![l5s07.png](images/l5s07.png)
![l5s08.png](images/l5s08.png)
![l5s09.png](images/l5s09.png)
