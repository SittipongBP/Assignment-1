# Assignment#1 การติดตั้ง Jenkins ใช้งานร่วมกับ GIT ,Python และ Robot Framework

<br>

### -:- **จัดทำโดย** : นายสิทธิพงศ์ บับพาน Section 1 รหัสนักศึกษา 613020029-1 -:-

<br>

## สิ่งที่ต้องเตรียมพร้อม และต้องติดตั้งให้เรียบร้อยก่อนใช้งาน มีดังนี้ <br>
    * Python Version 3.8.7
    * Java JDK 11.0.10
    * Robot Framework
    * Selenium Library
    * chromedriver_win32

<br><br>

## ------------------------------------------------------------------------------------------
## -:- ขั้นตอนการติดตั้ง Jenkins มีดังต่อไปนี้ -:-
## ------------------------------------------------------------------------------------------

<br>
<img src="image_jenkins/01.png" width="500"/>
<br>

- เข้าไปที่ Google Search แล้วค้นหาว่า Jenkins


<br>

<br>
<img src="image_jenkins/02.png" width="800"/>
<br>

- กดไปที่ Download


<br>

<br>
<img src="image_jenkins/03.png" width="800"/>
<br>

- ในที่นี้ใช้ระบบปฏิบัตการ Windows จึงทำการเลือกดาวน์โหลดในเวอร์ชัน Windows

<br>

<br>
<img src="image_jenkins/04.png" width="200"/>
<br>

- รอการดาวน์โหลดจนกว่าจะเสร็จสิ้น

<br>

<br>
<img src="image_jenkins/05.png" width="500"/>
<br>

- เมื่อดาวน์โหลดเสร็จสิ้น ให้คลิกติดตั้ง แล้วจะมีหน้าต่างขึ้นมาดังรูป
- แล้วกด Next

<br>

<img src="image_jenkins/06.png" width="500"/>
<br>

- ทำการเลือกที่ติดตั้ง ซึ่งระบบจะกำหนดมาให้แล้วในไดร์ C:
- แล้วกด Next

<br>

<img src="image_jenkins/07.png" width="500"/>
<br>

- ให้ทำการเลือก Run as service as LocalSystem เพราะจะติดตั้งไว้ที่เครื่องของเรา
- แล้วกด Next

<br>

<img src="image_jenkins/08.png" width="500"/>
<br>

- เลือก port (มีค่าตั้งแต่ 0-65535) แล้วทำการเทส
- เมื่อผ่านแล้ว ให้กด Next

<br>

<img src="image_jenkins/09.png" width="500"/>
<br>

- เลือกที่อยู่ของโฟลเดอร์ Java JDK เวอร์ชัน 11 ที่ติดตั้งไว้
- แล้วกด Next

<br>

<img src="image_jenkins/10.png" width="500"/>
<br>

- ขั้นตอนนี้ให้กด Next ไปเลย

<br>

<img src="image_jenkins/11.png" width="500"/>
<br>

- ให้ทำการติดตั้ง โดยการกด Install

<br>

<img src="image_jenkins/12.png" width="500"/>
<br>

- รอการติดตั้งสักครู่

<br>

<img src="image_jenkins/13.png" width="500"/>
<br>

- เสร็จสิ้นการติดตั้งแล้ว ให้ทำการกด Finish
- แล้วรอสักครู่ จะมีหน้าเว็บขึ้นมา

<br>



<img src="image_jenkins/14.png" width="800"/>
<br>

- เมื่อมีหน้าเว็บขึ้นมา ให้ทำการค้นหาไฟล์ Password ตามที่อยู่ตัวสีแดง
- แล้วทำการกรอก Password ลงไป

<br>

<img src="image_jenkins/15.png" width="800"/>
<br>

- ให้กดเลือก Install suggested plugins เพื่อทำการติดตั้ง plugin อัติโนมัติ ที่ระบบจัดหามาให้

<br>

<img src="image_jenkins/16.png" width="800"/>
<br>

- แล้วรอการติดตั้งสักครู่

<br>

<img src="image_jenkins/17.png" width="800"/>
<br>

- สำหรับการเข้าครั้งแรก ให้กรอกแบบฟอร์มตามที่กำหนดให้ถูกต้อง

<br>

<img src="image_jenkins/18.png" width="800"/>
<br>

- เมื่อเสร็จแล้ว จะมีหน้าแสดง URL + port ขึ้นมา ให้ทำการบันทึกไว้
- แล้วกด Save and Finish

<br>

<img src="image_jenkins/19.png" width="800"/>
<br>

- แล้วจะมีหน้าต่างบอกว่าพร้อมใช้งานแล้ว แสดงขึ้นมา
- แล้วกดไปที่ Start using Jenkins

<br>


## -:- การสร้างโปรเจคใน Jenkinds -:-
<br>

<img src="image_jenkins/20.png" width="800"/>
<br>

- เมื่อเข้ามาแล้ว ให้กดที่ Create a Job เพื่อสร้างไฟล์โปรเจคใหม่ขึ้นมา

<br>


## ------------------------------------------------------------------------------------------
## -:- การสร้างโปรเจคใน Jenkinds ร่วมกับการใช้ GIT -:-
## ------------------------------------------------------------------------------------------

<br>

<img src="image_jenkins/30.png" width="1000"/>
<br>

- ให้ตั้งชื่อโปรเจค โดยในที่นี้จะตั้งชื่อว่า Assignment1_jenkinds_GIT
- แล้วเลือก Freestyle Project
- แล้วกด Next

<br>

<br>

<img src="image_jenkins/31.png" width="1000"/>
<br>

- จะได้หน้าเพจแบบนี้ขึ้นมา
- ทำการ Configure เพื่อตั้งค่าโปรเจคของเรา

<br>

<img src="image_jenkins/32.png" width="1000"/>
<br>

- เลือกไปที่ Repository URL ที่อยู่ใต้แท็บ Source Code Management
- ให้ใส่ที่อยู่ Repository ของเราที่สร้างไว้ ซึ่งมีที่อยู่ว่า https://github.com/SittipongBP/Assignment-1

- แล้วตรง Branch ให้ใส่ตามที่ตั้งไว้ ซึ่งมีชื่อว่า */main
- แล้วกด Save

<br>

<img src="image_jenkins/33.png" width="1000"/>
<br>

- เมื่อทำการ Save แล้ว ให้กด Build Now เพื่อทดสอบผลการรันโปรแกรม
- แล้วคลิกเข้าไปที่ตัวเลขที่แสดงไว้ข้างวางกลมสีน้ำเงิน

<br>

<img src="image_jenkins/34.png" width="1000"/>
<br>

- แล้วกดเข้าไปที่ Console Output เพื่อดูผลการรัน

<br>

## ------------------------------------------------------------------------------------------
## -:- การสร้างโปรเจคใน Jenkinds ร่วมกับการใช้ภาษา Python -:-
## ------------------------------------------------------------------------------------------


<img src="image_jenkins/35.png" width="1000"/>
<br>

- ให้ตั้งชื่อโปรเจค โดยในที่นี้จะตั้งชื่อว่า Assignment1_jenkinds_Python
- แล้วเลือก Freestyle Project
- แล้วกด Next

<br>

<img src="image_jenkins/36.png" width="1000"/>
<br>

- แล้วกดออกมาที่หน้า Dashboard
- เข้าไปที่ Manage Jenkins 

<br>

<img src="image_jenkins/37.png" width="1000"/>
<br>

- เข้าไปที่ Manage Plugins เพื่อตั้งค่าหรือติดตั้ง Plugins ต่างๆเพิ่มเติม

<br>

<img src="image_jenkins/38.png" width="1000"/>
<br>

- ค้นหาคำว่า Python แล้วทำการติดตั้งทั้งหมด
- และ Restart Jenkins

<br>

<img src="image_jenkins/39.png" width="1000"/>
<br>

- เมื่อทำการติดตั้งเสร็จแล้ว ให้ทำการกดไปที่ config เพื่อตั้งค่าต่างๆ

<br>

<img src="image_jenkins/40.png" width="1000"/>
<br>

- ไปที่แท็บ Build แล้วเลือกตรงแถบข้างล่างว่า Execute Python Script
- ใส่ Code ภาษา python ลงไปเพื่อทำการทดสอบ

<br>

<img src="image_jenkins/41.png" width="1000"/>
<br>

- ทำการกด Build Now และคลิกเข้าไปที่ตัวเลขที่แสดงไว้ข้างวางกลมสีน้ำเงิน

<br>

<img src="image_jenkins/42.png" width="1000"/>
<br>

- ทำการกด Console Output เพื่อดูผลลัพธ์

<br>


## ------------------------------------------------------------------------------------------
## -:- การสร้างโปรเจคใน Jenkinds ร่วมกับการใช้ Robot Framework-:-
## ------------------------------------------------------------------------------------------

<br>
<img src="image_jenkins/43.png" width="1000"/>
<br>

- ให้ตั้งชื่อโปรเจค โดยในที่นี้จะตั้งชื่อว่า Assignment1_Robotframework
- แล้วเลือก Freestyle Project
- แล้วกด Next

<br>

<img src="image_jenkins/44.png" width="1000"/>
<br>

- เข้าไปที่ configure
- เลือกแท็บ Build
- แล้วไปที่ Build กดตรงที่ Execute Windows batch command
- Set path ที่ติดตั้ง Robot Framework และ Seleniun Library ไว้ เพื่อให้รันโปรแกรมได้
- เขียนคำสั่งเรียกใช้ไฟล์ .Robot โดยเรียกไฟล์ที่สร้างไว้ตาม path ที่เก็บข้อมูลไว้

<br>

<img src="image_jenkins/script.png" width="400"/>
<br>

- ตัวอย่าง code ในไฟล์ robot

<br>

<img src="image_jenkins/45.png" width="1000"/>
<br>

- ตั้งค่า path นำเอาข้อมูลผลการรันมาสร้างกราฟ
- ตั้งค่า % ในการพล็อตกราฟ
- แล้วกด Save

<br>

<img src="image_jenkins/46.png" width="300"/>
<br>

- แล้วกด Build Now

<br>

<img src="image_jenkins/47.png" width="1000"/>
<br>

- จะได้ผลการรันของ Robotframework ดังภาพข้างต้น
- คลิกเข้าไปที่ตัวเลขที่แสดงไว้ข้างวางกลมสีน้ำเงิน 

<br>

<img src="image_jenkins/48.png" width="1000"/>
<br>

- จะได้ผลลัพธ์ ดังนี้

<br>

<img src="image_jenkins/49.png" width="1000"/>
<img src="image_jenkins/50.png" width="1000"/>
<br>

- กดไปที่ Console Output เพื่อแสดงผลลัพธ์ที่ได้

<br>


<img src="image_jenkins/51.png" width="1000"/>
<br>

- ผลลัพธ์จากการทดสอบอื่นๆ ของ Robot Framework

<br>

<img src="image_jenkins/dashboard.png" width="1000"/>
<br>

- ผลลัพธ์รวมทั้งหมดจากหน้า Dashboard

<br>



