---
title: "3. ใบมีด + สกรู: ประกอบชิ้น"
parent: "C7 · เขียนแบบให้โรงงานอ่านออก: กบเหลา 3 ด้าน"
nav_order: 3
chapter: true
read_time: 3
do_time: 4
track: "📐 Engineering"
permalink: /courses/c7-measure-drafting/03-blade/
hook: "ทำชิ้นเล็กที่บางมาก (ใบมีดหนา 0.6 mm) ได้อย่างแม่นยำ และใช้ Screw/Bolt สร้างสกรูแบบมีเกลียวจาก preset"
---

# 3. ใบมีด + สกรู: ประกอบชิ้น
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำชิ้นเล็กที่บางมาก (ใบมีดหนา 0.6 mm) ได้อย่างแม่นยำ
- ใช้ **Screw/Bolt** สร้างสกรูแบบมีเกลียวจาก preset
- จัดชิ้นส่วนลง layer ตามวัสดุ (โลหะ / พลาสติก)

## 💡 ไอเดียสั้น ๆ
งาน engineering ต้องแยก **ชิ้นส่วน (part)** ให้ชัด เพราะแต่ละชิ้นผลิตต่างกัน: Body ทำจากพลาสติกฉีดหรือแมกนีเซียม, ใบมีดทำจากเหล็กปั๊ม, สกรูเป็นของสำเร็จรูป

| Part | วิธี | ค่า |
|---|---|---|
| Blade | Cube 18 × 9 × 0.6 วางบนหน้าบนเหนือช่อง | หนา 0.6 |
| รูสกรูบนใบมีด | Cylinder R1.25 + Difference | Ø2.5 |
| Screw | **Screw/Bolt** (Specialties) | M2.5 ยาว 5 |

## 👣 ลงมือทำ (4 นาที)
1. สร้าง **Blade** และเจาะรู Ø2.5
2. **Screw/Bolt** วางสกรูที่ศูนย์กลางรู (ปรับขนาดใน Tool Options)
3. **Layers**: `Plastic` (Body) · `Steel` (Blade, Screw)
4. ตั้งชื่อ `Blade` และ `Screw` แล้วบันทึก

{: .shot }
[SCREENSHOT: Screw/Bolt Tool Options]
{: .shot }
[SCREENSHOT: กบเหลา 3 ชิ้นประกอบกัน]

{: .verify }
พารามิเตอร์ของ **Screw/Bolt** (ขนาดเกลียว ความยาว ชนิดหัว) และความต่างระหว่าง Screw/Bolt กับ **Detailed Screw/Bolt** ใน v10 ต้องยืนยัน (คู่มือมีทั้งสองหน้า)

{: .shapr }
Shapr3D ไม่มีสกรูสำเร็จรูป (ต้องโหลดจาก McMaster-Carr) ส่วน formZ มี **Screw/Bolt** ในตัว

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** เปลี่ยนสกรูเป็นหัวแบน แล้ววัดความยาวรวมใหม่
</div>

📚 อ้างอิง: R1 Screw/Bolt, Detailed Screw/Bolt, Layers
