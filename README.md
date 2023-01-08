## Term Project || Go Camp

Go Camp เป็นแพลตฟอร์มการจองออนไลน์สำหรับสถานที่ตั้งแคมป์ในประเทศไทย 
ผู้ใช้สามารถค้นหาและจองพื้นที่ตั้งแคมป์ตามสถานที่ตั้ง ราคา และสิ่งอำนวยความสะดวก 
มันมีขั้นตอนการจองที่ง่ายและปลอดภัย

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
