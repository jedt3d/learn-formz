---
title: "SP4 · ที่วางมือถือบนโต๊ะ ใน 20 นาที"
parent: "⭐ Special Projects"
nav_order: 4
chapter: true
track: "📐 Engineering"
read_time: 2
do_time: 18
hook: "ทำที่วางมือถือเอียง 65° จากโปรไฟล์ 2D รูปเดียว"
permalink: /projects/sp4-phone-holder/
---

# SP4 · ที่วางมือถือบนโต๊ะ ใน 20 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **ที่วางมือถือบนโต๊ะ** จบใน 1 ครั้ง
- ฝึกซ้ำ: Line, Fit Fillet / Bevel, 3D Extrusion, Difference, Print Preparation

## 💡 ไอเดียสั้น ๆ
**งานสุดสัปดาห์** = ของชิ้นเล็ก 1 ชิ้น 20 นาที ใช้แค่สิ่งที่เรียนมาแล้ว · ต้องเรียนก่อน: **C2** · หน่วย mm

## 👣 ลงมือทำ (18 นาที)
1. วาดโปรไฟล์ด้านข้างด้วย **Line** (ฐาน 80, พนัก 100 เอียง 65°, ขอบกันลื่นสูง 12) บนระนาบ ZX
2. **Fit Fillet / Bevel** มุมทั้งหมด R3
3. **3D Extrusion** กว้าง 70
4. **Cylinder** Ø12 → **Difference** ช่องสายชาร์จ
5. **Print Preparation** แล้ว **Export STL**

{: .shot }
[SCREENSHOT: SP4 · ที่วางมือถือบนโต๊ะ ใน 20 นาที · ผลงานเสร็จ (render)]

{: .easy }
ทุกขั้นเป็นเครื่องมือที่เคยใช้แล้ว ถ้าลืมดู [Cheat sheet]({{ '/cheatsheet/' | relative_url }})

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** วัดความหนามือถือจริง + เคส แล้วปรับร่องให้พอดี (+0.5 mm)
</div>

📚 อ้างอิง: Manual: Line, Fit Fillet / Bevel, 3D Extrusion, Difference, Print Preparation
