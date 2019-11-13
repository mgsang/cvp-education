
# Arista Networks CVP Education

---
#### Arista Networks : 11월 12일 ~ 14일

---
#### 실습 가이드
<img src="https://drive.google.com/open?id=1erQfxUwqWxH9Prvdc_LJKZa6nh9YnwwZ" width="450px" height="300px"></img>

- Lab 접속 방법 : [arista01.showing.kr](http://arista01.showing.kr)
  - [lab-11](https://lab11.showing.kr)
  - [lab-12](https://lab12.showing.kr)
  - [lab-13](https://lab13.showing.kr)
  - [lab-14](https://lab14.showing.kr)
- Lab 접속 방법 : [arista02.showing.kr](http://arista02.showing.kr)
  - [lab-1](https://lab1.showing.kr)
  - [lab-2](https://lab2.showing.kr)
  - [lab-3](https://lab3.showing.kr)
  - [lab-4](https://lab4.showing.kr)


* CVP 설치 후 접속 방법<br>
https://121.138.134.{A}<br>
※ 192.168.200.A 마지막 A 를 입력

* dhcp 설정
~~~
subnet 10.183.0.0 netmask 255.255.255.0  {
        range 10.183.0.33 10.183.0.240;
        option bootfile-name "http://10.183.0.1/ztp/bootstrap";
} 
~~~

* dhcpd 시작
```
systemctl enable dhcpd.service 
systemctl start dhcpd.service 
```

* Configlet Import File<br>
[ExportedConfigletsData-7](https://drive.google.com/open?id=14zsCAc2TuIK8Aq76MpigYHi-RDR7WUx6)
