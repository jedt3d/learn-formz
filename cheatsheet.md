---
title: "📄 Cheat sheet A4"
nav_order: 84
permalink: /cheatsheet/
---

<div class="cheat" markdown="1">

# 📄 formZ 10 Cheat sheet (A4 · 2 หน้า)
{: .no_toc }
<p class="course-sub">พิมพ์ติดข้างจอ (Ctrl/Cmd + P → A4 → แนวตั้ง) · Win = Ctrl / Mac = Cmd</p>

{: .verify }
ปุ่มลัดในหน้านี้อิงจาก preset และคู่มือ formZ 10 ที่หาได้ ปุ่มที่มี 🔍 ให้ตรวจใน **Key Shortcuts** ของเครื่องตัวเองก่อนพิมพ์ เพราะแต่ละ edition หรือแต่ละคนตั้งค่าไม่เหมือนกัน

## 1. ตั้งครั้งเดียว ใช้ทุกวัน
- **Key Shortcuts › Load Defaults › Preset 2 = SketchUp** (Preset 1 = Rhino) → ปุ่มลัดเหมือน SketchUp ทันที
- ไม่รู้ว่าเครื่องมืออยู่ไหน? → **Keyword Assist** พิมพ์ชื่อเครื่องมือได้เลย 🔍
- ไม่รู้ต้องคลิกอะไรต่อ? → ดูบรรทัด **Assistant** ด้านล่างจอ
- **Taps** (กดปุ่มสั้น ๆ = สลับเครื่องมือ) vs **Quick Keys** (กดค้าง = ใช้ชั่วคราว ปล่อยแล้วกลับเครื่องมือเดิม) 🔍

## 2. ปุ่มที่ต้องจำ
| ทำอะไร | Win | Mac |
|---|---|---|
| Undo / Redo | Ctrl+Z / Ctrl+Shift+Z 🔍 | Cmd+Z / Cmd+Shift+Z 🔍 |
| Save / Save Incremental | Ctrl+S / 🔍 | Cmd+S / 🔍 |
| Copy / Paste | Ctrl+C / Ctrl+V | Cmd+C / Cmd+V |
| พิมพ์ค่าตัวเลขระหว่างใช้เครื่องมือ | Tab 🔍 | Tab 🔍 |
| สลับดู cage ของ SubD | F6 | F6 (อาจต้องกด fn) |
| หมุน / เลื่อน / ซูมมุมมอง | เมาส์กลาง / Shift+เมาส์กลาง / ล้อ 🔍 | เหมือนกัน หรือ trackpad 🔍 |

## 3. 30 เครื่องมือที่ใช้ 90% ของเวลา
| กลุ่ม | เครื่องมือ |
|---|---|
| ✏️ วาด 2D (6) | Line · Rectangle · Circle · Polygon · Spline · Text |
| 🧱 ขึ้นรูป (7) | 3D Extrusion · Revolve · Axial Sweep · Pipe · NURBS by Lofting · Skin · Cube / Cylinder / Sphere |
| ✂️ Boolean (3) | Union · Difference · Split |
| 🌀 มน / ผิว (5) | Controlled Round · Round · Round to Holdline · Fit Fillet / Bevel · Thicken |
| 🧸 ปั้น / ดัด (3) | Subdivision / Create · Radial Bend · Taper |
| ↔️ จัดวาง (4) | Move · Rotate · Scale · Mirror |
| 📏 ตรวจ / ผลิต (2) | Measure Distance · Print Preparation |

<div class="page-break"></div>

## 4. SketchUp / Shapr3D → formZ เร็ว ๆ
| เคยใช้ | ใน formZ |
|---|---|
| Push/Pull · Extrude | 3D Extrusion |
| Follow Me | Revolve · Axial Sweep · Pipe |
| Fillet (Shapr3D) | Controlled Round |
| Shell (Shapr3D) | Thicken / Shell 🔍 |
| Loft (Shapr3D) | NURBS by Lofting |
| Group / Component | Group / Components |
| History (Shapr3D) | ❌ ไม่มี history tree → ใช้ **Save Incremental** |
ดูครบที่ [Tool map]({{ '/tool-map/' | relative_url }})

## 5. ทำไม่ได้? เช็ก 5 ข้อก่อน
1. เครื่องมือเป็นสีเทา → edition ไม่รองรับหรือเปล่า? ([Editions]({{ '/editions/' | relative_url }}))
2. Boolean พัง → ชิ้นเป็น solid ไหม? ใช้ **Object Doctor**
3. Round error → รัศมีใหญ่เกินขอบ ลองค่าที่เล็กลง
4. ขนาดเพี้ยน 10× / 25.4× → หน่วย import ผิด ใช้ **Scale**
5. ทำพังแล้ว → เปิดไฟล์ **Save Incremental** เวอร์ชันก่อนหน้า

ดูเพิ่มที่ [Troubleshooting top-15]({{ '/troubleshooting/' | relative_url }})

## 6. Render เร็ว (RenderZone)
วัสดุ → แสง 1 Area + Environment → render ขนาดเล็กก่อน → ค่อยขยาย · ไม่ต้องใช้ Postprocess

</div>
