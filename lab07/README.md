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
API key is hidden
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
key hidden
![l7s13.png](images/l7s13.png)

```
$ sudo pip3 install -U gspread oauth2client
```
![l7s14.png](images/l7s14.png)

```
$ cd demo
$ cp ~/iot/lesson3/system_info.py .
$ cp ~/iot/lesson7/rpi_spreadsheet.py .
```
did not need system_info.py because I am doing a cpudata project
![l7s15.png](images/l7s15.png)

files properly copied to demo folder, key hidden
![l7s16.png](images/l7s16.png)

```
Start a new spreadsheet rpidata (or cpudata)
```
![l7s17.png](images/l7s17.png)

```
Share the spreadsheet with the "client_email" address in the .json file, select “Can edit,” and click "Send"
```
![l7s18.png](images/l7s18.png)

```
Delete Rows 2 to 1000, and enter Date / Time, CPU Usage %, Temperature C (or Memory Available GB for cpudata) to header cells
```
![l7s19.png](images/l7s19.png)
![l7s20.png](images/l7s20.png)

```
Edit rpi_spreadsheet.py
```
edited cpu_spreadsheet.py, key hidden
![l7s21.png](images/l7s21.png)

```
$ python3 rpi_spreadsheet.py
```
![l7s22.png](images/l7s22.png)

data properly collecting
![l7s23.png](images/l7s23.png)

[spreadsheet can be viewed by anyone with the link](https://docs.google.com/spreadsheets/d/1HkHynE6UBCzZVbJZs3Eoyt9ftPxSCAv70VdLFH6KNss/edit?usp=sharing)
![l7s24.png](images/l7s24.png)
