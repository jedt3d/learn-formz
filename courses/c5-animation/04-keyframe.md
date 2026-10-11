---
title: "4. Keyframe: เปิด-ปิดฝา"
parent: "C5 · Animation จากโมเดล"
nav_order: 4
chapter: true
read_time: 5
do_time: 5
permalink: /courses/c5-animation/04-keyframe/
---

# 4. Keyframe: เปิด-ปิดฝา
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ object ให้เป็น **animated entity** ด้วย **Keyframe** tool
- ใช้ **Auto Keyframe**: เลื่อนเวลา → ขยับของ → ได้ key ใหม่อัตโนมัติ
- ได้ฝาแม็กที่เปิด 30° แล้วปิดกลับใน 2 วินาที

## 💡 ไอเดียสั้น ๆ
**Keyframe** = "ภาพสำคัญ" ที่เราบอกว่า *ณ เวลานี้ ของต้องอยู่ตรงนี้* ส่วนระหว่างนั้น formZ จะเติมให้เอง (interpolation) ถ้าเปิด **Auto Keyframe** อยู่ ทุกครั้งที่แก้ของในเวลาใหม่ จะได้ key เพิ่มให้อัตโนมัติ (R5: The Animation Process)

| เวลา (วินาที) | สถานะของ UpperArm |
|---|---|
| 4.0 | ปิด (หลัง turntable จบ) |
| 5.0 | เปิด −30° |
| 6.0 | ปิด 0° |

## 👣 ลงมือทำ (5 นาที)
1. ลาก current time ไปที่ **4.0**
2. เลือก **Keyframe** tool แล้วคลิก `UpperArm` จะมีเส้นสีฟ้า (key) ขึ้นที่ไทม์ไลน์
3. ตรวจว่าเปิด **Auto Keyframe** อยู่ใน Time Line palette
4. ไปที่ **5.0** แล้วใช้ **Transform** หมุน UpperArm **−30°** รอบแกน Y (key ใหม่จะเกิดเอง)
5. ไปที่ **6.0** แล้วหมุนกลับ **+30°**
6. ลาก time ระหว่าง 4–6 เพื่อดู แล้วกด Play

{: .shot }
[SCREENSHOT: Time Line palette ที่มี 3 keys (4, 5, 6 วินาที) และไอคอน Auto Keyframe]
{: .shot }
[SCREENSHOT: ฝาเปิด 30° ที่เวลา 5.0]

{: .warning }
ถ้าเผลอขยับของตอนที่ time อยู่ที่ 0 ขณะเปิด Auto Keyframe อยู่ จะเกิด key ที่ไม่ต้องการ ให้ **Undo** หรือปิด Auto Keyframe ไว้ระหว่างจัดฉาก

{: .note }
ถ้าไม่ใช้ Auto Keyframe (manual) ให้ปิดไอคอนนั้น แล้วใช้ **Keyframe** tool คลิกซ้ำทุกครั้งหลังขยับของ (R5: The Keyframe Tool)

## ✅ เช็คตัวเอง
<details><summary>1. ระหว่าง key 2 อันเกิดอะไรขึ้น?</summary>formZ คำนวณตำแหน่งระหว่างกลางให้เอง (interpolation)</details>
<details><summary>2. Auto Keyframe ทำอะไร?</summary>สร้างหรืออัปเดต key อัตโนมัติเมื่อเราแก้ของในเวลาปัจจุบัน</details>
<details><summary>3. ทำไมเริ่มที่ 4.0 วินาที?</summary>เพราะ 0–4 วินาทีเป็นช่วง turntable</details>

📚 อ้างอิง: R5 The Animation Process, The Keyframe Tool, Swinging door tutorial
