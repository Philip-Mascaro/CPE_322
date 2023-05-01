note: will add copyable commands later

download GHDL and GTKWave according to instructions on [dsd repo](https://github.com/kevinwlu/dsd/tree/master/ghdl)
```
$ git clone https://github.com/kevinwlu/dsd.git
$ mkdir vhdl
$ cd vhdl
$ cp ~/dsd/ghdl/*vhdl .
```
![l1s01.png](images/l1s01.png)

```
$ ghdl -h
$ ghdl -v
$ ghdl -a hello.vhdl
$ ghdl -e hello_world
$ ghdl -r hello_world
```
![l1s02.png](images/l1s02.png)
![l1s03.png](images/l1s03.png)
![l1s04.png](images/l1s04.png)

Half Adder
```
$ ghdl -a ha.vhdl
$ ghdl -a ha_tb.vhdl
$ ghdl -e ha_tb
$ ghdl -r ha_tb --vcd=ha.vcd
$ gtkwave ha.vcd
```
![l1s05.png](images/l1s05.png)

import the variables and resize the axis using magnifier
![l1s06.png](images/l1s06.png)
![l1s07.png](images/l1s07.png)

window closing logged in command line
![l1s08.png](images/l1s08.png)

D Flip-Flop
```
$ ghdl -a dff.vhdl
$ ghdl -a dff_tb.vhdl
$ ghdl -e dff_tb
$ ghdl -r dff_tb --vcd=dff.vcd
$ gtkwave dff.vcd
```
![l1s09.png](images/l1s09.png)

import the variables and resize the axis using magnifier
![l1s10.png](images/l1s10.png)
![l1s11.png](images/l1s11.png)

window closing logged in command line
![l1s12.png](images/l1s12.png)
