---
title: "SP7 · จุกยางกันกระแทกประตู ใน 20 นาที"
parent: "⭐ Special Projects"
nav_order: 7
chapter: true
track: "🎨 Designer"
read_time: 2
do_time: 18
hook: "ปั้นจุกกันกระแทกทรงโดมนุ่ม ๆ ด้วย Subdivision"
permalink: /projects/sp7-bumper/
---

# SP7 · จุกยางกันกระแทกประตู ใน 20 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **จุกยางกันกระแทกประตู** จบใน 1 ครั้ง
- ฝึกซ้ำ: Subdivision / Create, Stretch, Offset Face, Convert Object Type, Difference

## 💡 ไอเดียสั้น ๆ
**งานสุดสัปดาห์** = ของชิ้นเล็ก 1 ชิ้น 20 นาที ใช้แค่สิ่งที่เรียนมาแล้ว · ต้องเรียนก่อน: **C3** · หน่วย mm

## 👣 ลงมือทำ (18 นาที)
1. **Cylinder** Ø40 H25 → **Subdivision / Create** Iterations 2
2. F6 ดู cage → ดึง face บนขึ้นให้เป็นโดม (**Stretch**)
3. **Offset Face** หน้าบนแล้วดันลง 2 mm เป็นร่องวงแหวน
4. **Convert Object Type** เป็น solid → **Cylinder** Ø5 **Difference** รูสกรู
5. วัสดุยางสีเทา + render

{: .shot }
[SCREENSHOT: SP7 · จุกยางกันกระแทกประตู ใน 20 นาที · ผลงานเสร็จ (render)]

{: .easy }
ทุกขั้นเป็นเครื่องมือที่เคยใช้แล้ว ถ้าลืมดู [Cheat sheet]({{ '/cheatsheet/' | relative_url }})

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำทรงหน้ายิ้มบนโดมด้วย Offset Face 3 จุด
</div>

📚 อ้างอิง: Manual: Subdivision / Create, Stretch, Offset Face, Convert Object Type, Difference
