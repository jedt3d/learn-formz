---
title: "1. แผนที่ความโค้ง: เลือกวิธีไหนดีใน 1 นาที"
parent: "M2 · 10 วิธีโค้งและมน ไม่ต้องลง plugin"
nav_order: 1
chapter: true
read_time: 3
do_time: 1
hook: "เลือกวิธีทำโค้ง/มนให้ถูกงานด้วยคำถาม 3 ข้อ"
permalink: /courses/m2-curves-rounds/01-map/
---

# 1. แผนที่ความโค้ง: เลือกวิธีไหนดีใน 1 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ตอบ 3 คำถามแล้วรู้ว่าควรใช้วิธีไหนใน 10 วิธี
- รู้ความต่างระหว่าง **มนขอบ** (rounding) กับ **สร้างผิวโค้ง** (surface)

## 💡 ไอเดียสั้น ๆ

| ถาม | ถ้าใช่ → | วิธี |
|---|---|---|
| มีกล่อง/ชิ้น solid อยู่แล้ว แค่อยากให้ขอบมน? | มนขอบ | 1 Controlled Round · 2 Round · 3 Round Between Faces · 4 Round to Holdline |
| ยังเป็นเส้น 2D อยู่? | มุมมนตั้งแต่ 2D | 5 Fit Fillet / Bevel |
| รูปทรงกลมรอบแกน / ตามเส้นทาง / เปลี่ยนหน้าตัด? | สร้างผิว | 6 Revolve · 7 Sweep + Pipe · 8 Skin + NURBS by Lofting |
| ฟอร์มอิสระแบบปั้นมือ? | ปั้น | 9 Subdivision |
| มีชิ้นงานแล้ว อยากดัด/บิด/เรียว? | deform | 10 Radial Bend · Twist · Taper |

## 👣 ลงมือทำ (1 นาที)
1. ดูของ 3 ชิ้นบนโต๊ะ แล้วเลือกวิธีให้แต่ละชิ้นจากตาราง
2. จดคำตอบไว้ แล้วตรวจอีกครั้งตอนจบ M2

{: .shot }
[SCREENSHOT: ตารางแผนที่ความโค้ง + ไอคอนเครื่องมือ 10 ตัว]

{: .power }
SketchUp ทำ 10 วิธีนี้ได้ในตัวไม่ถึงครึ่ง (ส่วนใหญ่ต้องลง extension เช่น RoundCorner, SubD, Curviloft, Shape Bender) ส่วน formZ มีครบในโปรแกรม

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ถ่ายภาพของในบ้าน 5 ชิ้นแล้วติดป้ายว่าใช้วิธีที่เท่าไร
</div>

## ✅ เช็คตัวเอง
<details><summary>1. กล่องที่อยากมนขอบ ใช้กลุ่มไหน?</summary>กลุ่มมนขอบ (วิธี 1–4)</details>
<details><summary>2. ขวดใช้วิธีไหน?</summary>Revolve (วิธี 6)</details>

📚 อ้างอิง: R1 Rounding, Derive, Deform, Subdivision
