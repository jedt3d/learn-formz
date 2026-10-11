---
title: "10. Slicer และพิมพ์จริง"
parent: "C8 · เตรียมผลิต: 3D Print, STEP"
nav_order: 10
chapter: true
read_time: 4
do_time: 7
track: "📐 Engineering"
permalink: /courses/c8-make-it/10-print/
---

# 10. Slicer และพิมพ์จริง
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปิด STL ใน **slicer** (เช่น PrusaSlicer, Cura, Bambu Studio) แล้วตั้งค่าพื้นฐาน
- **พิมพ์ทดสอบเกลียว** ก่อนพิมพ์ทั้งชิ้น (ประหยัดเวลาและเส้นพลาสติก)
- ปรับ clearance จากผลทดสอบ

## 💡 ไอเดียสั้น ๆ
Slicer อยู่ **นอก formZ** ทำหน้าที่หั่นโมเดลเป็นชั้น ๆ แล้วสร้างเส้นทางให้หัวพิมพ์

| ค่า | เริ่มที่ |
|---|---|
| Layer height | 0.2 mm (เกลียวเนียนขึ้นถ้าใช้ 0.12–0.16) |
| Walls / Perimeters | 3–4 (ผนัง 1.6 mm ≈ 4 เส้น) |
| Infill | 15–20 % |
| Support | ปิด (ถ้าไหล่ไม่เกิน 45° และกลับหัวฝาแล้ว) |
| วัสดุ | PLA |

**Test coupon:** ใน formZ ตัดเฉพาะคอขวดกับฝาส่วนบนออกมา (Difference ด้วยกล่อง) ให้สูงแค่ ~15 mm แล้วพิมพ์ทดสอบ ~20 นาที แทนที่จะพิมพ์ทั้งชิ้น 2 ชั่วโมง

## 👣 ลงมือทำ (7 นาที ไม่รวมเวลาพิมพ์)
1. ใน formZ: copy ขวดแล้วตัดเหลือเฉพาะคอ (z ≥ 64) → export `neck_test.stl`
2. ใน slicer: import `neck_test.stl` + `cap.stl` → ตั้งค่าตามตาราง → Slice แล้วดูเวลาและน้ำหนัก
3. ดู **preview ทีละชั้น** ที่เกลียว ว่ามีส่วนลอยไหม
4. พิมพ์แล้วลองขัน: **หลวมไป** ลด clearance เป็น 0.3 · **ฝืด/ขันไม่เข้า** เพิ่มเป็น 0.5 (กลับไปแก้บท 4)
5. ไม่มีเครื่องพิมพ์: ส่งภาพ preview จาก slicer เป็นการบ้านแทน

{: .shot }
[SCREENSHOT: slicer preview เห็นชั้นของเกลียว]
{: .shot }
[SCREENSHOT: ภาพถ่ายชิ้นทดสอบคอขวด + ฝาที่ขันเข้ากัน]

{% include homework.html id="c8-print" title="C8 · Bottle Cap Print" what="ภาพถ่ายฝาที่ขันเข้ากับคอขวด (หรือภาพ slicer preview) + ค่า clearance ที่ใช้" %}

{: .warning }
ถ้าใช้เครื่องพิมพ์ที่โรงเรียนหรือ FabLab ให้ทำตามกฎความปลอดภัยของที่นั่น เพราะหัวพิมพ์ร้อนประมาณ 200 °C

## ✅ เช็คตัวเอง
<details><summary>1. ทำไมต้องพิมพ์ test coupon?</summary>เพื่อทดสอบว่าเกลียวพอดีไหม โดยใช้เวลาและวัสดุน้อย</details>
<details><summary>2. ฝาขันไม่เข้า ต้องแก้ค่าอะไร?</summary>เพิ่ม clearance เช่นจาก 0.4 เป็น 0.5</details>
<details><summary>3. Slicer อยู่ใน formZ ไหม?</summary>ไม่อยู่ เป็นโปรแกรมแยก</details>

📚 อ้างอิง: R1 STL · R15 Export to STL for 3D printing
