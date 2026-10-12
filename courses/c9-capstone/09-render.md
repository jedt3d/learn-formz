---
title: "9. 2 สี 1 ภาพ hero"
parent: "C9 · Portfolio ชิ้นแรก: ของจากบ้านใน 90 นาที"
nav_order: 9
chapter: true
read_time: 4
do_time: 5
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/09-render/
renderzone: true
hook: "ทำ CMF 2 ชุดสี (Color · Material · Finish) และจัดสตูดิโอ 3 ไฟ + Environment (C4) แล้วเรนเดอร์ hero shot"
---

# 9. 2 สี 1 ภาพ hero
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **CMF** 2 ชุดสี (Color · Material · Finish)
- จัดสตูดิโอ 3 ไฟ + Environment (C4) แล้วเรนเดอร์ **hero shot**
- เรนเดอร์ภาพเทียบ 2 สีด้วยกล้องเดิม

## 💡 ไอเดียสั้น ๆ
| ชิ้น | ชุด A "Chalk" | ชุด B "Mango" |
|---|---|---|
| Shell + ปุ่ม | ขาวด้าน (Matte plastic) | เหลืองมะม่วงเงา |
| Base | เทาเข้ม | เทาเข้ม |
| Wheel | ยางดำ | ยางดำ |
| โลโก้ | Decal เทา | Decal ขาว |

**Hero shot** = ภาพหลักที่ขายไอเดีย: มุม 3/4 จากหน้าเยื้องข้างและต่ำเล็กน้อย, ไฟ Key ด้านซ้ายบน, ฉากหลังเรียบ

## 👣 ลงมือทำ (5 นาที)
1. สร้าง material ชุด A ตามตาราง (Duplicate จาก C4 ได้)
2. นำฉากสตูดิโอจาก C4 มาใช้ (ไฟ Area 3 ดวง + Environment) หรือ copy ไฟล์ฉากมาใช้
3. ตั้ง view hero แล้วบันทึกเป็น view ชื่อ `Hero` ใน **Views palette** (เหมือน C4)
4. **RenderZone** (Final Gather + AO ตามค่าใน C4 บท 10) → `mouse_A.png`
5. เปลี่ยนเป็นชุด B แล้วเรนเดอร์ภาพจาก view เดิม → `mouse_B.png`

{: .shot }
[SCREENSHOT: hero render ชุด A + ชุด B คู่กัน]

{: .warning }
อย่าเปิด **Postprocess** ของ RenderZone (มีรายงานว่าทำให้ 10.1.5 ค้าง) ถ้าอยากปรับภาพเพิ่ม ให้ใช้โปรแกรมแต่งภาพภายนอก

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำสีชุดที่ 3 ตามสีโปรดของเพื่อน
</div>

## ✅ เช็คตัวเอง
<details><summary>1. CMF ย่อมาจากอะไร?</summary>Color, Material, Finish</details>
<details><summary>2. ทำไมต้องใช้ view เดิมทั้ง 2 สี?</summary>ให้เปรียบเทียบได้ตรง ๆ</details>
<details><summary>3. Hero shot ถ่ายมุมไหน?</summary>มุม 3/4 จากหน้าเยื้องข้าง ต่ำเล็กน้อย</details>

📚 อ้างอิง: [C4]({{ '/courses/c4-renderzone-studio/' | relative_url }}) · R2 RenderZone
