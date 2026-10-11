---
title: "6. Place Frame: มุมมองที่ลิงก์กับโมเดล"
parent: "C6 · Brand & Presentation Boards"
nav_order: 6
chapter: true
read_time: 4
do_time: 4
permalink: /courses/c6-layout-boards/06-frame/
---

# 6. Place Frame: มุมมองที่ลิงก์กับโมเดล
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- วาง **frame** ที่แสดงโมเดล 3D แบบเส้น (hidden line) บน board
- เลือก **View** (Top / Front / Right ... หรือ view ที่บันทึกไว้) และ **Scale** หรือ **Fit**
- เลือก **Object Type** ของเส้น (Lines / Poly Lines / Lines, Splines and Arcs)

## 💡 ไอเดียสั้น ๆ
**Frame** คือ "หน้าต่าง" บนกระดาษที่มองเข้าไปในไฟล์โมเดล 3D ตาม view และมาตราส่วนที่ตั้งไว้ และ **ลิงก์อยู่ตลอด** ถ้าแก้โมเดลแล้ว frame อัปเดตได้ เส้นสวยแบบ line drawing ทำให้ board ดู "มีงานออกแบบจริง" ไม่ใช่แค่ภาพสวย (R1: Layout)

| Frame Parameters | ตั้งเป็น |
|---|---|
| File | `C3_Kettle.fmz` |
| View | **Front** (standard projection) |
| Scale | **Fit** (บน hero board) |
| Graphics > Object Type | **Lines, Splines and Arcs** (ไฟล์เล็ก + วัดรัศมีได้ใน C7) |
| Show Border | ปิด |

## 👣 ลงมือทำ (4 นาที)
1. เลือก **Place Frame** แล้วลากกรอบเล็ก ๆ ที่มุมขวาล่างของ `01_Hero`
2. ในหน้าต่าง **Frame Parameters** → File: ไอคอน Open → เลือกไฟล์กาต้มน้ำ
3. **Define Parameters**: View = Front · เปิด **Fit** · Object Type = Lines, Splines and Arcs · ปิด Show Border
4. กด **Options** (Hidden Line) แล้วเลือกให้ซ่อนเส้นด้านหลัง จากนั้นกด OK
5. ถ้าภาพไม่อยู่กลางกรอบ: Show Controls → กด **Cmd/Ctrl** แล้วลากเพื่อ re-center

{: .shot }
[SCREENSHOT: Frame Parameters dialog (File, View = Front, Fit, Object Type)]
{: .shot }
[SCREENSHOT: frame เส้นด้านหน้าของกาต้มน้ำบน hero board]

{: .power }
ใน SketchUp + LayOut ก็มี viewport ที่ลิงก์โมเดล แต่ต้องใช้ 2 โปรแกรม ส่วน formZ แปลงเป็น **เส้น vector แท้** (spline/arc) ซึ่งวัดขนาดต่อได้

## ✅ เช็คตัวเอง
<details><summary>1. Frame ต่างจาก Place Image อย่างไร?</summary>Frame ลิงก์กับโมเดล 3D และแสดงตาม view/scale ส่วน Image เป็นภาพนิ่งจากไฟล์</details>
<details><summary>2. ทำไมเลือก Lines, Splines and Arcs?</summary>ไฟล์เล็กกว่า และส่วนโค้งเป็น arc จริงที่วัดรัศมีได้</details>
<details><summary>3. Fit ทำอะไร?</summary>ย่อหรือขยายโมเดลให้พอดีกรอบโดยไม่สนมาตราส่วน</details>

📚 อ้างอิง: R1 Layout (Place Frame, Editing Frames), Hidden Line
