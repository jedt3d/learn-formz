---
title: "2. Product family: CMF เดียวกัน"
parent: "C6 · Brand & Presentation Boards"
nav_order: 2
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c6-layout-boards/02-family/
---

# 2. Product family: CMF เดียวกัน
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เข้าใจคำว่า **product family** และ **design language**
- ใช้ **CMF ชุดเดียวกัน** (สี วัสดุ ผิว) กับกาต้มน้ำและแก้วมัค
- เรนเดอร์ภาพ **ชุด** 2 ภาพสำหรับ board

## 💡 ไอเดียสั้น ๆ
สินค้าในชุดเดียวกันต้อง **ดูเป็นครอบครัวเดียวกัน** ด้วย 3 อย่าง:

| ภาษาออกแบบ | กาต้มน้ำ | แก้วมัค |
|---|---|---|
| **รูปทรง** | ไหล่โค้ง, ก้นป่อง | ก้นป่องนิด ๆ แบบเดียวกัน |
| **รายละเอียด** | หูจับสีดำ | หูจับสีดำ |
| **CMF** | `KT_Steel` + `KT_Plastic_Black` | เซรามิกขาว + หูจับ `KT_Plastic_Black` |

## 👣 ลงมือทำ (5 นาที)
1. เปิด `C3_Kettle.fmz` แล้ว copy แก้วมัคมาวาง (File > Import หรือ copy/paste)
2. ใช้ material เดิมของกากับหูจับแก้ว แล้วทำ `MG_Ceramic_White` (Glossy ขาว) ให้ตัวแก้ว
3. จัดวาง: แก้วอยู่หน้า-ขวาของกา หันหูจับไปทางเดียวกัน
4. ใช้แสงสตูดิโอจาก C4 แล้วเรนเดอร์ **2 ภาพ**:
   - `C6_Family_Hero.png`: ภาพ 2 ชิ้นคู่กัน แนวนอน 2400 × 1500
   - `C6_Detail.png`: ภาพซูมหูจับ แนวตั้ง

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์ family hero (กา + แก้ว)]

{: .note }
ถ้ามีเวลา ให้ทำ **ฉากหลังสีเดียวกับแบรนด์** (Background สี pastel) จะทำให้ board ดูกลมกลืนขึ้น

📚 อ้างอิง: R3 Materials · C4 แสงสตูดิโอ
