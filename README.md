
# Arista Networks CVP Education

---
#### Arista Networks : 11월 12일 ~ 14일

---
## 실습 가이드
<img src="./education_map.jpg">

- Lab 접속 방법 : [arista01.showing.kr](http://arista01.showing.kr)
  - Lab CVP 접속 방법 : 
    - [lab-11](https://lab11.showing.kr)
    - [lab-12](https://lab12.showing.kr)
    - [lab-13](https://lab13.showing.kr)
    - [lab-14](https://lab14.showing.kr)
- Lab 접속 방법 : [arista02.showing.kr](http://arista02.showing.kr)
  - Lab CVP 접속 방법 : 
    - [lab-1](https://lab-1.showing.kr)
    - [lab-2](https://lab-2.showing.kr)
    - [lab-3](https://lab-3.showing.kr)
    - [lab-4(Reserved)](https://lab-4.showing.kr)

* Configlet Import File<br>
[ExportedConfigletsData-7](https://drive.google.com/open?id=14zsCAc2TuIK8Aq76MpigYHi-RDR7WUx6)


--- 
## Pre-Installation
* Installation Complete with CVP Single node 
## Pre-Configuration

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

---
Appendix.
* Software Download tab
https://www.arista.com/en/support/software-download

* CloudVision Portal (CVP) Setup
https://www.arista.com/en/cg-cv/cv-cloudvision-portal-cvp-setup


