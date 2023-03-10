## Term Project || Go Camp

Go Camp เป็นแพลตฟอร์มการจองออนไลน์สำหรับสถานที่ตั้งแคมป์ในประเทศไทย 
ผู้ใช้สามารถค้นหาและจองพื้นที่ตั้งแคมป์ตามสถานที่ตั้ง ราคา และสิ่งอำนวยความสะดวก 
มันมีขั้นตอนการจองที่ง่ายและปลอดภัย
  วัตถุประสงค์ของการทำระบบจองเต็นท์ เพื่อตอบสนองกลุ่มใช้งานทั่วไปที่อยากใช้เวลาในวันหยุดไป
  พักผ่อนแต่ไม่รู้ว่าจะไปที่ไหนหรืออยากไปสถานที่ใหม่ๆแต่ยังไม่สามารถเลือกสถานที่ที่จะไปได้ทาง
  เราจึงได้เก็บรวบรวมสถานที่บ้านพักรีสอร์ทหรือสถานที่ลับๆที่เงียบสงบทางเราจึงสร้างเว็ปนี้เพื่อตอบ
  สนองความต้องการของผู้ใช้แต่ละประเภท
## Database Design

ระบบของเรามีตาราง 2 ตารางได้แก่ User ที่จะเก็บเอาข้อมูลสำหรับการทำระบบ login อย่างง่ายและตารางข้อมูลการจองที่พักที่จะประกอบไปด้วยข้อมูลที่เป็นรายละเอียดต่าง ๆ ของการจอง ดังตัวอย่างที่จะกล่าวต่อไปนี้


## ตัวอย่างตาราง User และ JSON
| id | UserID | password | isLogged |
| ----- | ----- | ----- | ----- |
| 1 | admin | admin | false |
| 2 | admin1 | admin1 | false |

#### ตัวอย่าง JSON

```json
"Users": [
    {
      "UserID": "admin",
      "isLogged": "false",
      "password": "admin",
      "id": 1
    },
    {
      "UserID": "admin1",
      "password": "admin1",
      "isLogged": "false",
      "id": 2
    }
]
```

## ตัวอย่างตาราง Booking และ JSON

| UserID | parkName   | checkIn    | checkOut   | paymentStatus | HowManyPerson | id  |
| ------ | ---------- | ---------- | ---------- | ------------- | ------------- | --- |
| admin  | รวงข้าว  | 2023-01-07 | 2023-01-08 | ⌛ pending     | 1             | 1   |
| admin1 | admin1Data | 2023-01-07 | 2023-01-09 | ❌ unpaid      | 1             | 2   |

#### ตัวอย่าง JSON

```json
"Booking": [
    {
      "UserID": "admin",
      "parkName": "รวงข้าว",
      "checkIn": "2023-01-07",
      "checkOut": "2023-01-08",
      "paymentStatus": "⌛ pending",
      "HowManyPerson": "1",
      "id": 1
    },
    {
      "UserID": "admin1",
      "parkName": "admin1Data",
      "checkIn": "2023-01-07",
      "checkOut": "2023-01-09",
      "paymentStatus": "❌ unpaid",
      "HowManyPerson": "1",
      "id": 2
    }
  ]

```
## 🔗 Links to youtube
คลิกโลโก้youtubeเพื่อไปยังคำอธิบายฟังก์ชั่น
[![youtube](https://www.youtube.com/img/desktop/yt_1200.png)](https://youtu.be/5P_od3m8jO4)
# RWD
อธิบายเกี่ยวกับRWD
computer
![Logo](https://sv1.picz.in.th/images/2023/01/08/JD9a0I.jpg)
####
####
iphone 12 Pro
####
แนวนอน
![Logo](https://sv1.picz.in.th/images/2023/01/08/JDkNG0.jpg)
####
แนวตั้ง
![Logo](https://sv1.picz.in.th/images/2023/01/08/JDkLut.jpg)
####
iped air
####
แนวตั้ง
![Logo](https://sv1.picz.in.th/images/2023/01/08/JD3mxJ.jpg)
####
แนวนอน
![Logo](https://sv1.picz.in.th/images/2023/01/08/JD3MKa.jpg)
## 🔗 สมาชิก
#### 64108749 ปิยากร อินทร์ฉาย
#### 64117260 สหรัฐ ศรีสว่าง
#### 64121080 อาภัสรา โสดาพัฒน์
