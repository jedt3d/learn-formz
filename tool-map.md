---
title: "🔁 SketchUp / Shapr3D → formZ"
nav_order: 81
permalink: /tool-map/
---

# เคยใช้ SketchUp หรือ Shapr3D? หาเครื่องมือที่คุ้นเคยใน formZ ได้ใน 1 นาที
{: .no_toc }

ใช้ **Ctrl+F / Cmd+F** หาชื่อเครื่องมือที่รู้จัก แล้วกดลิงก์ไปบทที่สอน ชื่อฝั่ง formZ ใช้ชื่อ official ของ formZ 10 ถ้าหาไม่เจอในเมนู ให้พิมพ์ชื่อใน **Assistant** (C1 บท 1)

<details markdown="1"><summary>สารบัญ</summary>

- TOC
{:toc}
</details>

## 1. SketchUp → formZ

| SketchUp | formZ 10 | เรียนที่ | หมายเหตุ |
|---|---|---|---|
| Select (Space) | **Pick** + topological level (object/face/segment/point) | [C2-3]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }}) | เลือกระดับก่อนแล้วค่อยคลิก |
| Line (L) | **Vector Line** | [C2-4]({{ '/courses/c2-solid-form/04-profile/' | relative_url }}) | |
| Rectangle (R) | **Rectangle** | [C2-2]({{ '/courses/c2-solid-form/02-base/' | relative_url }}) | เลือก object type เป็น solid ได้ทันที |
| Circle (C) / Polygon | **Circle** / **Polygon** | [C3-2]({{ '/courses/c3-curves-surfaces/02-pencil/' | relative_url }}) | |
| Arc (A) | **Arc** | [C2-4]({{ '/courses/c2-solid-form/04-profile/' | relative_url }}) | |
| **Push/Pull (P)** | **3D Extrusion** (สร้าง) · **Reshape** (ดึงหน้าเดิม) | [C2-2]({{ '/courses/c2-solid-form/02-base/' | relative_url }}) · [C2-3]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }}) | 🟢 ความรู้สึกเหมือนกัน |
| Follow Me | **Sweep** (Axial / Two Source) · **Pipe** | [C6-1]({{ '/courses/c6-layout-boards/01-mug/' | relative_url }}) | |
| Offset (F) | **Thicken** (ผนัง solid) | [C2-9]({{ '/courses/c2-solid-form/09-thicken/' | relative_url }}) | 🔍 การ offset เส้น 2D ให้ดูใน manual |
| Move (M) / Rotate (Q) / Scale (S) | **Move** / **Rotate** / **Scale** (กลุ่ม Transform) | [C2-6]({{ '/courses/c2-solid-form/06-align/' | relative_url }}) | copy ด้วย tap Alt/Option ([M1-3]({{ '/courses/m1-quick-tips/03-taps/' | relative_url }})) |
| Tape Measure (T) | **Measure Distance** + **Draw Guide** | [C7-4]({{ '/courses/c7-measure-drafting/04-measure/' | relative_url }}) · [M1-4]({{ '/courses/m1-quick-tips/04-guides/' | relative_url }}) | |
| Protractor | **Measure Angle** | [C7-4]({{ '/courses/c7-measure-drafting/04-measure/' | relative_url }}) | |
| Dimensions | **Linear / Multi / Radial / Angular Dimension** | [C7-6]({{ '/courses/c7-measure-drafting/06-linear/' | relative_url }}) | dimension ตามโมเดล (Associativity) |
| Text / 3D Text | **Text** + 3D Extrusion | [C9-7]({{ '/courses/c9-capstone/07-details/' | relative_url }}) | 🔍 ฟอนต์ไทย |
| Paint Bucket (B) | **Materials palette** (ลากใส่ object/face) | [C1-6]({{ '/courses/c1-quick-win/06-materials/' | relative_url }}) | |
| Eraser (E) | **Delete** (เลือกแล้วกด Delete) | – | |
| Groups | **Group** | [C2-10]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | |
| Components | **Components** / **Component Manager** | [M1-6]({{ '/courses/m1-quick-tips/06-place-on/' | relative_url }}) | |
| Tags (Layers) | **Layers** | [C2-10]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | |
| Outliner | **Objects palette** | [C2-10]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | |
| Solid Tools: Union / Subtract / Intersect / Split | **Union / Difference / Intersection / Split** | [C1-5]({{ '/courses/c1-quick-win/05-details/' | relative_url }}) · [C3-3]({{ '/courses/c3-curves-surfaces/03-sharpen/' | relative_url }}) · [C2-7]({{ '/courses/c2-solid-form/07-split/' | relative_url }}) | 🚀 SketchUp ต้องใช้ Pro |
| Section Plane | **Clipping Plane** / **Section** | [C7-8]({{ '/courses/c7-measure-drafting/08-section/' | relative_url }}) | |
| Scenes | **Views palette** | [C1-3]({{ '/courses/c1-quick-win/03-view/' | relative_url }}) | |
| Styles / Face Style | Display modes (Wire Frame, Shaded ...) | [C1-3]({{ '/courses/c1-quick-win/03-view/' | relative_url }}) | |
| Match Photo | **Matching Views To Pictures** | (แผนใน M1) | 🔍 |
| Search (Shift+S) | **Assistant** / Keyword Assist | [C1-1]({{ '/courses/c1-quick-win/01-start/' | relative_url }}) | |
| Keyboard shortcuts | **Key Shortcuts › Load Defaults › Preset 2** (แบบ SketchUp) | [M1-1]({{ '/courses/m1-quick-tips/01-shortcuts/' | relative_url }}) | 🟢 |
| LayOut | **formZ Layout** | [C6]({{ '/courses/c6-layout-boards/' | relative_url }}) | Pro |
| 3D Warehouse | Component Manager libraries | – | ไม่มีคลังออนไลน์ใหญ่เท่า 3D Warehouse |
| Extension: RoundCorner | **Controlled Round** (ในตัว) | [C1-5]({{ '/courses/c1-quick-win/05-details/' | relative_url }}) · [C2-8]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }}) | 🚀 |
| Extension: SubD / Vertex Tools | **Subdivision** (ในตัว) | [C3-8]({{ '/courses/c3-curves-surfaces/08-subd-intro/' | relative_url }}) | 🚀 |
| Extension: Curviloft | **NURBS by Lofting** / **Tangent Loft** / **Skin** | [C3-6]({{ '/courses/c3-curves-surfaces/06-loft/' | relative_url }}) · [C8-2]({{ '/courses/c8-make-it/02-body/' | relative_url }}) | 🚀 |
| Extension: Solid Inspector | **Print Preparation** + **Object Doctor** | [C8-6]({{ '/courses/c8-make-it/06-print-prep/' | relative_url }}) · [C8-7]({{ '/courses/c8-make-it/07-doctor/' | relative_url }}) | 🚀 |
| Render extension (V-Ray, Enscape ...) | **RenderZone** (plugin ของ formZ) | [C4]({{ '/courses/c4-renderzone-studio/' | relative_url }}) | |
| Scenes animation | **Animation** (Turntable, Keyframe, Staging) | [C5]({{ '/courses/c5-animation/' | relative_url }}) | 🚀 Pro |

## 2. Shapr3D → formZ

| Shapr3D | formZ 10 | เรียนที่ | หมายเหตุ |
|---|---|---|---|
| Sketch บนระนาบ | **Reference plane** (XY / YZ / ZX) + เครื่องมือ 2D | [C1-2]({{ '/courses/c1-quick-win/02-setup/' | relative_url }}) | |
| Extrude | **3D Extrusion** | [C2-2]({{ '/courses/c2-solid-form/02-base/' | relative_url }}) | |
| ดึงหน้า (direct modeling) | **Reshape** | [C2-3]({{ '/courses/c2-solid-form/03-pick-reshape/' | relative_url }}) | |
| Revolve | **Revolve** | [C3-5]({{ '/courses/c3-curves-surfaces/05-revolve/' | relative_url }}) | |
| Sweep | **Sweep** / **Pipe** | [C6-1]({{ '/courses/c6-layout-boards/01-mug/' | relative_url }}) | |
| Loft | **NURBS by Lofting** / **Tangent Loft** (Caps = solid) | [C3-6]({{ '/courses/c3-curves-surfaces/06-loft/' | relative_url }}) · [C8-2]({{ '/courses/c8-make-it/02-body/' | relative_url }}) | |
| Fillet | **Controlled Round** / **Round** | [C2-8]({{ '/courses/c2-solid-form/08-rounds/' | relative_url }}) | |
| Shell | **Thicken** | [C2-9]({{ '/courses/c2-solid-form/09-thicken/' | relative_url }}) | |
| Union / Subtract / Intersect | **Union / Difference / Intersection** | [C1-5]({{ '/courses/c1-quick-win/05-details/' | relative_url }}) | |
| Split body | **Split** | [C2-7]({{ '/courses/c2-solid-form/07-split/' | relative_url }}) | |
| Mirror | **Mirror** / **Object Symmetry** | [C2-10]({{ '/courses/c2-solid-form/10-organize/' | relative_url }}) | |
| Measure | **Measure Distance / Between / Quantities** | [C7-4]({{ '/courses/c7-measure-drafting/04-measure/' | relative_url }}) | |
| Drawings | **Layout**: frame 3 ด้าน + dimension | [C7-9]({{ '/courses/c7-measure-drafting/09-views/' | relative_url }}) | Pro |
| Visualization | **RenderZone** | [C1-8]({{ '/courses/c1-quick-win/08-render/' | relative_url }}) | |
| Export STEP / STL | **STEP / STL** | [C8-8]({{ '/courses/c8-make-it/08-stl/' | relative_url }}) · [C8-9]({{ '/courses/c8-make-it/09-step/' | relative_url }}) | |
| ประวัติการแก้ไข (ถ้าใช้) | **ไม่มี history tree** ให้ใช้ **controlled/parametric objects** + **File › Save Incremental** | [C1-2]({{ '/courses/c1-quick-win/02-setup/' | relative_url }}) | ⚠ ความต่างที่สำคัญที่สุด |
| ปั้นด้วย Pencil บน iPad | เมาส์ + ปุ่มลัด + Taps | [M1]({{ '/courses/m1-quick-tips/' | relative_url }}) | formZ ทำงานบน Mac/Windows |

{: .note }
🟢 = ง่ายเหมือนเดิม · 🚀 = SketchUp ทำในตัวไม่ได้หรือต้องลง extension · 🔍 = ยังต้องยืนยันบนหน้าจอจริง
