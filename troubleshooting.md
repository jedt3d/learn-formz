---
title: "🛟 แก้ปัญหา 15 อันดับ"
nav_order: 82
permalink: /troubleshooting/
---

# แก้ปัญหา 15 อันดับ: อาการ → สาเหตุ → วิธีแก้
{: .no_toc }

ติดอยู่? ไม่ต้องเริ่มใหม่ ลองไล่จากตารางนี้ก่อน **ทุกครั้งก่อนแก้ ให้กด File › Save Incremental** (formZ ไม่มี history tree จึงควรมีไฟล์เวอร์ชันไว้ย้อนกลับ) ถ้ายังไม่หาย ให้ถามที่ forum official https://forums.formz.com/ (แนบภาพหน้าจอ + บอกเลขเวอร์ชันจาก Help › About)

<details markdown="1"><summary>สารบัญ</summary>

- TOC
{:toc}
</details>

## 🧱 ปั้นโมเดล

### 1. Boolean (Union / Difference) ไม่ผ่าน หรือได้ผลแปลก ๆ
- **สาเหตุ:** ผิวของ 2 ชิ้น **ซ้อนกันพอดี** (coplanar), ชิ้นใดชิ้นหนึ่งไม่ใช่ solid, หรือเป็น object ต่างชนิดกัน
- **แก้:** ① ขยับตัวตัดให้ **ทะลุออกไป 0.1–1 mm** ② ตรวจด้วย **Object Doctor** ③ ถ้าเป็น smooth กับ facetted ปนกัน ให้ใช้ **Convert Object Type** ให้เป็นชนิดเดียวกัน
- เรียนที่: [C1-5]({{ '/courses/c1-quick-win/05-details/' | relative_url }}) · [C8-7]({{ '/courses/c8-make-it/07-doctor/' | relative_url }})

### 2. Controlled Round ไม่ผ่าน / ขอบหาย
- **สาเหตุ:** รัศมี **ใหญ่กว่า** ขอบหรือหน้าที่อยู่ติดกัน, หรือ round หลายขอบที่มาชนกันที่มุมพร้อมกัน
- **แก้:** ลดรัศมีลงครึ่งหนึ่ง แล้วทำ **ทีละกลุ่มขอบ** (ขอบยาวก่อน ขอบสั้นทีหลัง) ถ้าต้องการขอบตามเส้น ใช้ **Round to Holdline**
- เรียนที่: [C2-8]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }})

### 3. Thicken แล้ว error หรือผนังทะลุ
- **สาเหตุ:** ความหนามากกว่ารัศมีความโค้งที่แคบที่สุดของผิว
- **แก้:** ลดความหนา, Thicken ไปทางนอกแทนด้านใน, หรือลดรัศมี round ก่อน Thicken
- เรียนที่: [C2-9]({{ '/courses/c2-solid-form/09-thicken/' | relative_url }})

### 4. คลิกแล้วเลือกผิด (ได้ทั้งชิ้นแทนที่จะได้หน้า)
- **สาเหตุ:** topological level ไม่ถูก
- **แก้:** เลือกระดับ (Object / Face / Segment / Point) ก่อน แล้วค่อยคลิก
- เรียนที่: [C2-3]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }})

### 5. วาดแล้วชิ้นงานไปอยู่ผิดระนาบ / ลอยกลางอากาศ
- **สาเหตุ:** reference plane ไม่ใช่ระนาบที่ตั้งใจ (เช่น ยังอยู่ที่ ZX)
- **แก้:** เปลี่ยนกลับเป็น **XY** แล้วใช้ object snap กับพื้นผิว หรือแตะ **Ctrl/Cmd** (taps) ระหว่างลาก
- เรียนที่: [C1-2]({{ '/courses/c1-quick-win/02-setup/' | relative_url }}) · [M1-3]({{ '/courses/m1-quick-tips/03-taps/' | relative_url }})

### 6. ขนาดเพี้ยน 10 / 25.4 / 1000 เท่า
- **สาเหตุ:** หน่วยของโปรเจกต์ไม่ใช่ mm หรือไฟล์ที่ import มาใช้หน่วยอื่น
- **แก้:** ตรวจหน่วยใน **Project Settings** ให้เป็น mm แล้ว **Measure Distance** ด้านที่รู้ขนาดจริง ถ้าผิด ใช้ **Scale** ด้วยตัวคูณ (เช่น 25.4 สำหรับนิ้ว → mm)
- เรียนที่: [C1-2]({{ '/courses/c1-quick-win/02-setup/' | relative_url }})

## 🖥️ หน้าจอและโปรแกรม

### 7. เครื่องมือหาย / palette หาย (โดยเฉพาะบน Mac หลังอัปเดต)
- **สาเหตุ:** workspace เดิมไม่รู้จักเครื่องมือใหม่ (มีรายงานใน 10.1.x)
- **แก้:** **Workspace › Reset Workspace** แล้วเปิดโปรแกรมใหม่ และอัปเดตเป็นเวอร์ชันล่าสุด
- เรียนที่: [แหล่งอ้างอิง]({{ '/references/' | relative_url }})

### 8. หาเครื่องมือไม่เจอ
- **แก้:** พิมพ์ชื่อใน **Assistant** หรือดู [ตารางเทียบเครื่องมือ]({{ '/tool-map/' | relative_url }})

### 9. หมุนมุมมองแล้วงง / ชิ้นงานหายไปจากจอ
- **แก้:** ใช้คำสั่งดูทั้งหมด (zoom all/extents) จากเมนู View แล้วเลือกมุมที่บันทึกไว้ใน **Views palette** ถ้ามือยังไม่ชิน ให้ใช้ **Key Shortcuts › Preset 2** (แบบ SketchUp)
- เรียนที่: [C1-3]({{ '/courses/c1-quick-win/03-view/' | relative_url }}) · [M1-1]({{ '/courses/m1-quick-tips/01-shortcuts/' | relative_url }})

{: .verify }
ชื่อคำสั่ง zoom all ในเมนู View ของ 10.1.x ต้องยืนยัน

## 🎨 วัสดุและ Render

### 10. Render แล้วโปรแกรมค้าง / ปิดตัวเอง
- **สาเหตุที่พบบ่อย:** เปิด **Postprocess** ของ RenderZone (มีรายงานว่า crash บน 10.1.5), ความละเอียดภาพสูงเกิน, GI quality สูงเกิน
- **แก้:** **ปิด Postprocess**, render ขนาด 1280 px ก่อน, ลด quality แล้วค่อยเพิ่ม และกด Save Incremental ก่อน render
- เรียนที่: [C1-8]({{ '/courses/c1-quick-win/08-render/' | relative_url }}) · [C4-10]({{ '/courses/c4-renderzone-studio/10-gi-shots/' | relative_url }})

### 11. ภาพมืด / แบน / ดูไม่จริง
- **แก้ 3 จุด:** ① มุมกล้อง (เลนส์ยาวขึ้น ต่ำลงนิดหนึ่ง) ② ไฟ Key + Fill + Rim ③ วัสดุที่มี Reflection และ Bump
- เรียนที่: [C4-8]({{ '/courses/c4-renderzone-studio/08-area-light/' | relative_url }}) · [C4-3]({{ '/courses/c4-renderzone-studio/03-shaders/' | relative_url }})

### 12. Texture ยืด / ลายใหญ่หรือเล็กเกิน
- **แก้:** ตรวจ Mapping Type แล้วปรับขนาดด้วย **Edit Texture**
- เรียนที่: [C4-6]({{ '/courses/c4-renderzone-studio/06-texture/' | relative_url }})

## 🏭 ผลิตและส่งไฟล์

### 13. Print Preparation เตือน Non Solids / Thin Objects
- **แก้:** ลบเส้น 2D หรือโปรไฟล์ที่เหลือ, ซ่อมด้วย **Object Doctor** (Fix If Possible), ผนังต้อง ≥ 1.2 mm
- เรียนที่: [C8-6]({{ '/courses/c8-make-it/06-print-prep/' | relative_url }})

### 14. ไฟล์ STL ใหญ่มาก / เกลียวเป็นเหลี่ยม
- **แก้:** แปลงเป็น facetted ที่ความละเอียดพอดี แล้วใช้ **Simplify Mesh** ด้วย Target Number Triangles (~150,000)
- เรียนที่: [C8-8]({{ '/courses/c8-make-it/08-stl/' | relative_url }})

### 15. ฟอนต์ไทยไม่ขึ้นใน Text / Layout
- **แก้:** ลองใช้ฟอนต์ไทยที่ติดตั้งในระบบ (เช่น Sarabun, Noto Sans Thai) ถ้าสระลอยหรือตัด ให้ทำเป็นภาพ PNG แล้ว **Place Image** แทน
- เรียนที่: [C6-7]({{ '/courses/c6-layout-boards/07-brand/' | relative_url }})

{: .verify }
การแสดงผลภาษาไทยใน Text tool และ Layout ของ formZ 10 ยังไม่ได้ทดสอบ
