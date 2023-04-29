```
$ sudo pip3 install numpy scipy scikit-learn matplotlib pandas tensorflow keras
```
installations done using Anaconda Navigator


```
$ cd ~/demo
$ cp ~/iot/lesson8/plt_final.py .
$ cp ~/iot/lesson8/plt_cv2.py .
```
before command
![l8s01.png](images/l8s01.png)
after command
![l8s02.png](images/l8s02.png)

```
$ nano plt_final.py
$ nano plt_cv2.py
```
update the data series and the chart titles\
1. plt_final.py:
   - data = read_csv('cpudata - Sheet1.csv')
2. plt_cv2.py:
   - X = read_csv('cpudata - Sheet1.csv', usecols=[1])
   - y = read_csv('cpudata - Sheet1.csv', usecols=[2])

![l8s03.png](images/l8s03.png)
![l8s04.png](images/l8s04.png)
![l8s05.png](images/l8s05.png)


```
$ python3 plt_final.py
$ python3 plt_cv2.py
```
![l8s06.png](images/l8s06.png)

Figure 1\
cannot see Memory Available GB series well\
![l8s07.png](images/l8s07.png)

Figure 1 larger\
can now see Memory Available GB series well\
![l8s08.png](images/l8s08.png)

Figure 2
![l8s09.png](images/l8s09.png)

Figure 3
![l8s10.png](images/l8s10.png)

Figure 4
![l8s11.png](images/l8s11.png)

Figure 5
![l8s12.png](images/l8s12.png)

Figure 6
![l8s13.png](images/l8s13.png)

Figure 7
![l8s14.png](images/l8s14.png)
