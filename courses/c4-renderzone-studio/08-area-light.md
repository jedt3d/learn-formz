---
title: "8. ไฟสตูดิโอ 3 ดวง: Key · Fill · Rim"
parent: "C4 · ถ่ายสินค้าแบบสตูดิโอ: เครื่องปิ้งขนมปัง 3 มุม"
nav_order: 8
chapter: true
read_time: 4
do_time: 5
permalink: /courses/c4-renderzone-studio/08-area-light/
hook: "เปลี่ยนแผ่นสี่เหลี่ยมให้เป็น Area light (เหมือน softbox ในสตูดิโอถ่ายภาพ) และจัด แสง 3 จุด: Key · Fill · Rim"
---

# 8. ไฟสตูดิโอ 3 ดวง: Key · Fill · Rim
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- เปลี่ยนแผ่นสี่เหลี่ยมให้เป็น **Area light** (เหมือน softbox ในสตูดิโอถ่ายภาพ)
- จัด **แสง 3 จุด**: Key · Fill · Rim
- ตั้งความสว่างเป็น **lumens/watts**

## 💡 ไอเดียสั้น ๆ
แสงจุด (point, cone, distant) ออกจาก **จุดเล็กมาก** เงาจึงคม ส่วน **Area light** ออกจาก **ผิวของวัตถุ** ทั้งแผ่น เงาจึงนุ่ม และโลหะจะสะท้อนเป็น **แถบสว่างสวย ๆ** (R3: Area and Line Lights)

| ไฟ | ตำแหน่ง | ขนาดแผ่น | หน้าที่ |
|---|---|---|---|
| **Key** | หน้าเฉียงซ้าย สูงกว่าเครื่อง | 600 × 400 | แสงหลัก |
| **Fill** | ขวา ต่ำกว่า | 400 × 400 · แรงครึ่งหนึ่งของ Key | ลดเงาดำ |
| **Rim** | ด้านหลังบน | 800 × 150 (แถบยาว) | เส้นขอบสว่างแยกจากฉากหลัง |

## 👣 ลงมือทำ (5 นาที)
1. วาด **Rectangle** (type 2D surface) ขนาด Key แล้วหมุนให้หันหน้าเข้าหาเครื่อง (Rotate บนระนาบที่เหมาะสม)
2. **Pick** แผ่นนั้นไว้ → สร้างไฟใหม่ใน **Lights** palette → ใน Light Parameters ที่ **Type** เลือก **Area**
3. ตั้งค่า intensity (เริ่มที่ประมาณ 1000 lumens แล้วปรับ) และเปิด shadows
4. ทำซ้ำกับ Fill และ Rim
5. ปิดไฟ distant เดิมจาก C1 (หรือลดลง) แล้วลองเรนเดอร์ทดสอบ
6. ซ่อนแผ่นไฟไม่ให้เห็นในภาพ ถ้าค่าใน Area light มีตัวเลือกนี้ หรือจัดให้อยู่นอกกรอบกล้อง

{: .shot }
[SCREENSHOT: Light Parameters dialog: Type = Area + Area Light options]
{: .shot }
[SCREENSHOT: มุมมองบน (Top) เห็นตำแหน่งไฟ Key / Fill / Rim รอบเครื่องปิ้ง]

{: .verify }
ช่องปรับ intensity และตัวเลือก "ไม่แสดงแผ่นไฟในภาพ" ของ Area light ใน v10 ต้องยืนยันบนเครื่องจริง · อย่าเปิด **Glow** เพราะจะเห็นเป็นก้อนแสงในภาพ

{: .note }
ตารางในคู่มือ: หลอดไส้ 100 W ≈ 1,380 lumens · หลอดฟลูออเรสเซนต์ 40 W ≈ 1,900–3,400 lumens ใช้เป็นจุดเริ่มต้นได้ (R3: Specifying The Correct Light Intensity)

{: .power }
SketchUp **ไม่มีไฟ** เลย (มีแค่แสงอาทิตย์สำหรับเงา) ส่วน formZ + RenderZone มีไฟหลายชนิด รวมถึง area/line light จากวัตถุจริง

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ปิด Fill light แล้ว render ภาพแบบ dramatic 1 ภาพ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ทำไม area light ให้เงานุ่ม?</summary>เพราะแสงออกจากผิวขนาดใหญ่ ไม่ใช่จุดเล็ก ๆ</details>
<details><summary>2. Rim light มีไว้ทำอะไร?</summary>ทำเส้นขอบสว่าง แยกตัวสินค้าออกจากฉากหลัง</details>
<details><summary>3. ต้องเลือกอะไรก่อนสร้าง area light?</summary>Pick วัตถุที่จะเป็นแผ่นไฟ</details>

📚 อ้างอิง: R3 Area and Line Lights, Making Lights Glow, Specifying The Correct Light Intensity
