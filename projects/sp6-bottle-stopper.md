---
title: "SP6 · ฝาขวดกันหก ใน 20 นาที"
parent: "⭐ Special Projects"
nav_order: 6
chapter: true
track: "📐 Engineering"
read_time: 2
do_time: 18
hook: "ทำฝาจุกขวดน้ำทรงโค้ง มีปีกจับ และพิมพ์ 3D ได้"
permalink: /projects/sp6-bottle-stopper/
---

# SP6 · ฝาขวดกันหก ใน 20 นาที
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- ทำ **ฝาขวดกันหก** จบใน 1 ครั้ง
- ฝึกซ้ำ: Spline, Revolve, Union, Round Between Faces, Print Preparation

## 💡 ไอเดียสั้น ๆ
**งานสุดสัปดาห์** = ของชิ้นเล็ก 1 ชิ้น 20 นาที ใช้แค่สิ่งที่เรียนมาแล้ว · ต้องเรียนก่อน: **C3 (ดีถ้าผ่าน C8)** · หน่วย mm

## 👣 ลงมือทำ (18 นาที)
1. วัดปากขวดจริงด้วยไม้บรรทัด/เวอร์เนียร์ (เช่น Ø ใน 22 mm)
2. วาดโปรไฟล์ครึ่งเดียวด้วย **Spline**: ส่วนเสียบเรียว Ø21.6 → 20.5 (เผื่อ 0.4), หัวโค้ง Ø30
3. **Revolve** รอบแกน Z
4. **Cube** แผ่นปีก 30 × 4 × 14 → **Union** → **Round Between Faces** R2
5. **Print Preparation** → **Export STL** พิมพ์ด้วย TPU ถ้ามี

{: .shot }
[SCREENSHOT: SP6 · ฝาขวดกันหก ใน 20 นาที · ผลงานเสร็จ (render)]

{: .easy }
ทุกขั้นเป็นเครื่องมือที่เคยใช้แล้ว ถ้าลืมดู [Cheat sheet]({{ '/cheatsheet/' | relative_url }})

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** ทำรูระบายอากาศ Ø1 ตรงกลาง แล้วดูว่าน้ำไหลออกง่ายขึ้นไหม
</div>

📚 อ้างอิง: Manual: Spline, Revolve, Union, Round Between Faces, Print Preparation
