---
title: "4. New Layout Project: A3"
parent: "C6 · Brand & Presentation Boards"
nav_order: 4
chapter: true
read_time: 4
do_time: 3
permalink: /courses/c6-layout-boards/04-new-layout/
---

# 4. New Layout Project: A3
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- สร้าง layout ด้วย **File > New Layout Project**
- ตั้ง **Units / Standard Paper Size / Landscape / Margin / Border**
- จัดการหลายแผ่นด้วย **Sheets** palette

## 💡 ไอเดียสั้น ๆ
**Layout** คือ "โหมดกระดาษ 2D" ใน formZ ไว้วางมุมมองของโมเดล 3D ตามมาตราส่วน และ **ลิงก์กับโมเดล** เมื่อโมเดลเปลี่ยน layout ก็อัปเดตได้ ไฟล์ layout เป็น **.fml** (R1: Layout)

| ค่า (New Layout dialog) | ตั้งเป็น |
|---|---|
| Name | `C6_KitchenSet_Boards` |
| Units | **Centimeters** หรือหน่วย metric (ค่าเริ่มต้นตามเครื่อง) |
| Standard Paper Size | **A3** |
| Landscape | ✅ |
| Margin | 10 mm |
| Border | ✅ Weight บาง |

## 👣 ลงมือทำ (3 นาที)
1. **File > New Layout Project** ตั้งค่าตามตาราง แล้วกด OK จะได้แผ่นที่ 1
2. workspace จะเปลี่ยนเป็นชุดเครื่องมือของ Layout (บางเมนูจะเป็นสีเทา เป็นเรื่องปกติ)
3. **Sheets** palette: เปลี่ยนชื่อแผ่นแรกเป็น `01_Hero` แล้วกด **Add** เพิ่มแผ่น `02_Views`
4. คลิกคอลัมน์แรกเพื่อสลับแผ่น active (จุดแดง) แล้วบันทึก

{: .shot }
[SCREENSHOT: New Layout dialog (A3, Landscape, Margin, Border)]
{: .shot }
[SCREENSHOT: Sheets palette ที่มี 01_Hero และ 02_Views]

{: .note }
แก้ขนาดกระดาษภายหลังได้ที่ **File > Project Settings > Layout** แต่ถ้าเปลี่ยนหลังวางของแล้ว ของบนแผ่นอาจเคลื่อน

{: .power }
SketchUp ต้องใช้ **LayOut** ซึ่งเป็นอีกโปรแกรมแยกต่างหาก ส่วน formZ มี Layout อยู่ในโปรแกรมเดียวกัน

## ✅ เช็คตัวเอง
<details><summary>1. ไฟล์ layout นามสกุลอะไร?</summary>.fml</details>
<details><summary>2. ทุกแผ่นในโปรเจกต์ใช้ขนาดกระดาษเดียวกันไหม?</summary>ใช่</details>
<details><summary>3. แผ่นไหนคือแผ่นที่ active?</summary>แผ่นที่มีจุดแดงใน Sheets palette</details>

📚 อ้างอิง: R1 Layout (R6)
