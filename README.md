
# Arista Networks CVP Education

---
#### Arista Networks : 11월 12일 ~ 14일

---
#### 실습 가이드

- Lab 접속 방법 : arista01.showing.kr
  - [lab-11](lab11.showing.kr)
  - [lab-12](lab12.showing.kr)
  - [lab-13](lab13.showing.kr)
  - [lab-14](lab14.showing.kr)
  - [lab-15](lab15.showing.kr)

- Telnet Program
  - [Windows Download](https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe)


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
