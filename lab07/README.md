```
Sign up and log in ThingSpeak
Create new channel cpu_loop with field1 cpu_pc and field2 mem_avail_mb
Copy the Write API Key from channels
```
![l7s01.png](images/l7s01.png)

```
$ sudo pip3 install -U psutil
```
![l7s02.png](images/l7s02.png)

```
$ cd ~/demo
$ cp ~/iot/lesson7/thingspeak_cpu_loop.py .
$ cp ~/iot/lesson7/thingspeak_feed.py .
```
![l7s03.png](images/l7s03.png)

```
$ cat thingspeak_cpu_loop.py
```
![l7s04.png](images/l7s04.png)

```
$ cat thingspeak_feed.py
```
![l7s05.png](images/l7s05.png)

```
$ python3 thingspeak_feed.py
An API key savefile was not found. Enter Write API Key >>>
Should we save this key for future use? [y/N] >>>
```
![l7s06.png](images/l7s06.png)

data collected
![l7s07.png](images/l7s07.png)

data collected again
![l7s08.png](images/l7s08.png)

```
Click "Create" and enter the project name, e.g., rpidata
```
did cpudata
![l7s09.png](images/l7s09.png)

```
≡ > APIs & Services > + Enable APIs & Services > Enable both Drive API and Sheets API
```
![l7s10.png](images/l7s10.png)
![l7s11.png](images/l7s11.png)

```
Credential > Create Credentials > Create service account key > Service account > rpidata > JSON key type > Create > download rpidata-xxxxxxxxxxxx.json
```
![l7s12.png](images/l7s12.png)
![l7s13.png](images/l7s13.png)

```
$ sudo pip3 install -U gspread oauth2client
```
![l7s14.png](images/l7s14.png)

ghghgh
![l7s15.png](images/l7s15.png)
![l7s16.png](images/l7s16.png)
![l7s17.png](images/l7s17.png)
![l7s18.png](images/l7s18.png)
![l7s19.png](images/l7s19.png)
![l7s20.png](images/l7s20.png)
![l7s21.png](images/l7s21.png)
![l7s22.png](images/l7s22.png)
![l7s23.png](images/l7s23.png)
![l7s24.png](images/l7s24.png)
