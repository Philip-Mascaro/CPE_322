note: will add copyable commands later
```
$ cd ~/iot/lesson10
$ cat hash_value.py
$ python3 hash_value.py
$ python3 hash_value.py
```
![l10s01.png](images/l10s01.png)

```
$ cd ~/iot/lesson10
$ cat snakecoin.py
$ python3 snakecoin.py
```
![l10s02.png](images/l10s02.png)

```
$ cat snakecoin-server-full-code.py
$ python3 snakecoin-server-full-code.py
$ cd
```
note: the final cd command will bring the user to the home directory
![l10s03.png](images/l10s03.png)

```
$ curl "localhost:5000/txion" \
     -H "Content-Type: application/json" \
     -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
$ curl localhost:5000/mine
```
![l10s04.png](images/l10s04.png)
![l10s05.png](images/l10s05.png)
![l10s06.png](images/l10s06.png)
![l10s07.png](images/l10s07.png)
![l10s08.png](images/l10s08.png)
![l10s09.png](images/l10s09.png)

```
Uncomment the last line of node_server.py
```
```
$ git clone https://github.com/satwikkansal/python_blockchain_app.git
$ cd ~/python_blockchain_app
$ nano node_server.py
```
![l10s10.png](images/l10s10.png)
![l10s11.png](images/l10s11.png)
```
$ python3 node_server.py
```
![l10s12.png](images/l10s12.png)

```
$ vncserver
$ cd ~/python_blockchain_app
$ python3 run_app.py
```
![l10s13.png](images/l10s13.png)

```
Via VNC viewer, open a browser on Raspberry Pi and go to YourNet running at http://127.0.0.1:5000/

Enter content and name, click "Post," and click "Request to mine" that generate "Block #1 is mined" at http://127.0.0.1:8000/mine

At YourNet, click "Resync" to view Block #1
```
![l10s14.png](images/l10s14.png)
![l10s15.png](images/l10s15.png)
![l10s16.png](images/l10s16.png)
