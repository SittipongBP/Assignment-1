# การติดตั้ง Jenkins #

## ขั้นตอนที่ 1 ติดตั้ง Java ##

<br>
<img src="image_jenkins/java 1.png" width="800"/>
<br>

* ให้เข้าไปที่เว็บไซต์ https://www.oracle.com/java เพื่อทำการ Download Java JDK 
* ให้คลิกเลือกที่ JDK Download
<br><br>

<img src="image_jenkins/java 2.png" width="800"/>
<br>

* กรณีนี้เป็นระบบปฎิบัติการ Windows 64bit จึงต้องทำการเลือก Windows x64 Installer
<br><br>

<img src="image_jenkins/java 3.png" width="800"/>
<br>

* กดปุ่ม / และทำการกด Download
<br><br>

<img src="image_jenkins/java 4.png" width="300"/>
<br>

* รอการ Download
<br><br>

<img src="image_jenkins/java 5.png" width="500"/>
<br>

* เมื่อ Download เสร็จแล้ว จะทำการติดตั้ง ให้กด Next
<br><br>

<img src="image_jenkins/java 6.png" width="500"/>
<br>

* เลือกที่สำหรับติดตั้ง และกด Next
<br><br>

<img src="image_jenkins/java 7.png" width="500"/>
<br>

* รอการติดตั้ง
<br><br>

<img src="image_jenkins/java 8.png" width="500"/>
<br>

* เมื่อติดตั้งเสร็จแล้ว ให้กด close แล้วทำการ set path ตามขั้นตอนต่อไป
<br><br>

<img src="image_jenkins/java 9.png" width="800"/>
<br>

* ทำการ copy path ที่ลง Java JDK ไว้ แล้วนำมาวางไว้ที่ path environment   ตามขั้นตอนต่อไป
<br><br>

<img src="image_jenkins/java 10.png" width="800"/>
<br>

* เมื่อเข้าไปที่ path แล้วให้กด New และทำการวาง path ลงไป แล้วกด OK
<br><br><br><br>

## ขั้นตอนที่ 2 ติดตั้ง Jenkins ##
<br>

<img src="image_jenkins/1.png" width="800"/>
<br>

* เข้าไปที่ www.jenkins.io
<br><br>

<img src="image_jenkins/2.png" width="800"/>
<br>

* คลิกที่ Download
<br><br>

<img src="image_jenkins/3.png" width="800"/>
<br>

* กรณีนี้เป็นระบบปฎิบัติการ Windows จึงต้องทำการเลือก Windows 
<br><br>

<img src="image_jenkins/4.png" width="300"/>
<br>

* รอการ Download
<br><br>

<img src="image_jenkins/5.png" width="500"/>
<br>

* เมื่อ Download เสร็จ จะทำการติดตั้งโดยการกด Next
<br><br>

<img src="image_jenkins/6.png" width="500"/>
<br>

* เลือกที่ติดตั้ง และกด Next ต่อไป
<br><br>

<img src="image_jenkins/7.png" width="500"/>
<br>

* เลือก Run service as LocalSystem และกด Next
<br><br>

<img src="image_jenkins/8.png" width="500"/>
<br>

* ให้สร้าง port 8080 และกด Test Port เพื่อทดสอบว่าใช้ได้หรือไม่ 
* เมื่อผ่านแล้วให้ทำการกด Next
<br><br>

<img src="image_jenkins/9.png" width="500"/>
<br>

* ให้ add path ของ Java JDK เข้ามา
<br><br>

<img src="image_jenkins/10.png" width="500"/>
<br>

* เมื่อเสร็จแล้วให้กด Finish แล้วรอสักครู่ จะมี Browser โผล่ขึ้นมาให้ทำการตั้งค่า
<br><br><br><br>

## ขั้นตอนที่ 3 ตั้งค่า Jenkins ##
<br>

<img src="image_jenkins/11.png" width="800"/>
<br>

* ทำการใส่ Administrator Password โดยนำมาจากที่อยู่ตามตัวหนังสือสีแดงข้างบน
<br><br>

<img src="image_jenkins/12.png" width="800"/>
<br>

* เมื่อผ่านแล้วให้ทำการเลือก Install Suggested Plugins คือการติดตั้งปลั๊กอินแบบอัตโนมัติ
<br><br>

<img src="image_jenkins/13.png" width="800"/>
<br>

* รอการติดตั้ง Plugin สักครู่
<br><br>

<img src="image_jenkins/14.png" width="800"/>
<br>

* ทำการสร้าง Account ตามแบบฟอร์ม และกด Save & Continue
<br><br>


<img src="image_jenkins/15.png" width="800"/>
<br>

* ระบบจะสร้าง URL ให้อัตโนมัติ และให้ทำการ Save & Finish
<br><br>


<img src="image_jenkins/16.png" width="800"/>
<br>

* ติดตั้งเสร็จแล้ว เริ่มการใช้งานโดยคลิกไปที่ Start using Jenkins
<br><br><br><br>

## ขั้นตอนที่ 4 การทำให้ Jenkins ทำงานควบคู่กับ Git ได้ ##
<br>

<img src="image_jenkins/17.png" width="800"/>
<br>

* เริ่มสร้างโปรเจคโดยกกดไปที่ Create a job
<br><br>


<img src="image_jenkins/18.png" width="800"/>
<br>

* ตั้งชื่อ ( ตั้งชื่อว่า Assignment_Jenkins_Git ) และคลิกเลือก Freestyle Project
<br><br>



