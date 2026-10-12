---
title: "10. ส่งงานครบชุด 4 ไฟล์"
parent: "C9 · Portfolio ชิ้นแรก: ของจากบ้านใน 90 นาที"
nav_order: 10
chapter: true
read_time: 4
do_time: 6
track: "🎨 Designer + 📐 Engineering"
permalink: /courses/c9-capstone/10-deliver/
edition: pro
hook: "ทำ บอร์ด A3 1 แผ่นใน Layout (C6) และทำ แบบ 3 ด้าน + dimension หลัก (C7)"
---

# 10. ส่งงานครบชุด 4 ไฟล์
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **บอร์ด A3** 1 แผ่นใน **Layout** (C6)
- ทำ **แบบ 3 ด้าน** + dimension หลัก (C7)
- Export **PDF + STEP + STL** ให้ครบชุด (C8)

## 💡 ไอเดียสั้น ๆ
**ชุดส่งงาน (deliverables):**

| ไฟล์ | ทำจาก | ใช้กับ |
|---|---|---|
| `mouse_board.pdf` (A3) | Layout: Place Image (hero A/B) + Place Frame + Text | portfolio |
| `mouse_drawing.pdf` (A4) | Layout: frame 3 ด้าน + Linear/Radial Dimension + title block | วิศวกร |
| `mouse.step` (AP214) | ไฟล์ smooth | CAD อื่น |
| `mouse_shell.stl` ... | ไฟล์ facetted | พิมพ์ต้นแบบ |

**บอร์ด:** หัวเรื่อง + hero ใหญ่ (50%) + 2 สี + exploded 4 ชิ้น + Zebra + brief 3 บรรทัด

## 👣 ลงมือทำ (6 นาที)
1. **New Layout Project** A3 → วาง hero, ภาพสี B, exploded (render ใหม่ หรือ Place Frame)
2. **Place Text**: ชื่อสินค้า + ไอเดีย 1 ประโยคจาก brief + swatch สี
3. sheet ใหม่ A4: **Place Multi-Frame** 3 ด้าน, scale 1:1 → Linear Dimension ยาว/กว้าง/สูง + Radial ของล้อ → title block จาก C7
4. Export PDF ทั้ง 2 sheet
5. Export STEP (AP214) จากไฟล์ smooth และ STL จากไฟล์ facetted

{: .shot }
[SCREENSHOT: บอร์ด A3 สุดท้าย]
{: .shot }
[SCREENSHOT: แบบ A4 3 ด้าน]

{% include homework.html id="c9-capstone" title="C9 · Capstone" what="บอร์ด A3 (PDF หรือภาพ) + hero render + ภาพของจริงที่ใช้อ้างอิง" %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ใส่ QR code ของลิงก์วิดีโอ turntable ลงในบอร์ด
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ส่งงานให้วิศวกรต้องมีอะไร?</summary>แบบ PDF + ไฟล์ STEP</details>
<details><summary>2. hero ควรกินพื้นที่บอร์ดเท่าไร?</summary>~50%</details>
<details><summary>3. STL export จากไฟล์ไหน?</summary>ไฟล์ facetted</details>

📚 อ้างอิง: [C6]({{ '/courses/c6-layout-boards/' | relative_url }}) · [C7]({{ '/courses/c7-measure-drafting/' | relative_url }}) · [C8]({{ '/courses/c8-make-it/' | relative_url }})
