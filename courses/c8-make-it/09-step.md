---
title: "9. ส่งไฟล์ให้ CAD อื่น + ชั่งน้ำหนัก"
parent: "C8 · พิมพ์ 3D ให้ขันได้จริง: ขวด + ฝาเกลียว"
nav_order: 9
chapter: true
read_time: 4
do_time: 3
track: "📐 Engineering"
permalink: /courses/c8-make-it/09-step/
hook: "รู้ว่า STEP ต่างจาก STL อย่างไร และควรใช้เมื่อไร และExport STEP แบบ AP214 (ค่าเริ่มต้น) หรือ AP203"
---

# 9. ส่งไฟล์ให้ CAD อื่น + ชั่งน้ำหนัก
{% include meta.html %}

## 🎯 จบบทนี้แล้วเราจะ...
- รู้ว่า **STEP** ต่างจาก STL อย่างไร และควรใช้เมื่อไร
- Export STEP แบบ **AP214** (ค่าเริ่มต้น) หรือ **AP203**
- ใช้ **Mass Properties** ประมาณน้ำหนักชิ้นพิมพ์จาก density

## 💡 ไอเดียสั้น ๆ
| | STL | STEP |
|---|---|---|
| เก็บอะไร | สามเหลี่ยม (โดยประมาณ) | **ผิว NURBS/solid แบบแม่นยำ** (ISO 10303) |
| ใช้กับ | slicer / เครื่องพิมพ์ | **โปรแกรม CAD อื่น** (Shapr3D, Fusion, SolidWorks), โรงงานทำแม่พิมพ์ |
| แก้ต่อได้ไหม | ยาก | ได้ (ยังเป็น solid) |

Solid จะ export เป็น STEP ชนิด **MANIFOLD_SOLID_BREP** (หรือ BREP_WITH_VOIDS ถ้ามีช่องว่างข้างใน) และเปิดในโปรแกรมอื่นได้เป็น solid (R1: STEP)

## 👣 ลงมือทำ (3 นาที)
1. เปิด **ไฟล์ smooth** (`C8_Bottle.fmz`) → **File › Export...** → **STEP** → Schema **AP214** → `bottle_cap.step`
2. (ถ้ามี Shapr3D) ลอง import ไฟล์ STEP ดู จะได้ solid ที่วัดขนาดได้ ✅
3. **Mass Properties** → คลิก `Cap` → ตั้ง density ของ **PLA ≈ 1.24 g/cm³** แล้วอ่าน Weight
4. เทียบกับ **Measure Quantities** (C7) ว่า Volume ตรงกันไหม
5. จดน้ำหนักขวด + ฝา เพื่อใช้ประมาณค่าเส้นพลาสติกในบทหน้า

{: .shot }
[SCREENSHOT: Export STEP Schema AP214]
{: .shot }
[SCREENSHOT: Mass Properties palette: Weight And Volume]

{: .note }
น้ำหนักที่ได้คือของ **ชิ้นตัน 100%** ส่วน slicer ใช้ infill (เช่น 20%) ชิ้นพิมพ์จริงจึงเบากว่า แต่ชิ้นที่ผนังบาง (1.6 mm) ส่วนใหญ่เป็นผนังล้วน จึงใกล้เคียงค่าที่คำนวณ

{: .verify }
STEP export จากไฟล์ smooth ส่ง NURBS แบบแม่นยำจริงไหม หรือแปลงเป็น facet ก่อน และตำแหน่งที่ตั้ง density ใน Mass Properties ต้องยืนยันใน v10

{: .power }
SketchUp export STEP ไม่ได้ (ต้องใช้ extension) ส่วน formZ export STEP **ในตัว** จึงคุยกับโปรแกรม engineering ได้

{% include can-sketchup.html id=8 %}

<div class="challenge" markdown="1">
🏆 **ท้าทาย 5 นาที:** คำนวณว่าเส้น PLA 1 kg พิมพ์ขวดได้กี่ใบ
</div>

## ✅ เช็คตัวเอง
<details><summary>1. ส่งไฟล์ให้โรงงานทำแม่พิมพ์ควรใช้อะไร?</summary>STEP</details>
<details><summary>2. Schema ค่าเริ่มต้นคืออะไร?</summary>AP214</details>
<details><summary>3. ทำไมน้ำหนักจริงอาจน้อยกว่า Mass Properties?</summary>เพราะ slicer ใช้ infill ไม่ได้พิมพ์ตัน 100%</details>

📚 อ้างอิง: R1 STEP, Mass Properties, Measure Quantities
