---
title: "🎁 โจทย์เสริม: Pebble Speaker"
parent: "C1 · Quick Win"
nav_order: 99
permalink: /courses/c1-quick-win/bonus-speaker/
---

# 🎁 โจทย์เสริม: Pebble Speaker
<div class="meta-bar"><span>🛠 ลงมือ ~25 นาที</span><span>ใช้ความรู้จาก C1 บท 4–8</span></div>

ลำโพงบลูทูธจิ๋วทรงกระบอก ขอบโค้งมน มีวัสดุ 3 แบบ (ตัวเครื่องด้าน, ฝายาง, ปุ่มโลหะ)

| ชิ้น | วิธีทำ | ขนาด |
|---|---|---|
| Body | Cylinder Preset | Radius 35, Height 80 ที่ (0,0,0) |
| ขอบ Body | Controlled Round 2 sets | บน R6 · ล่าง R3 |
| Cap | Cylinder Preset บนหน้าบน (Snap to Center) | Radius 27, Height 2 |
| ร่องปุ่ม | Cylinder R6 H2 วางบน Cap แล้ว Move ลง 1 mm → **Difference** (คลิก Cap ก่อน) | Ø12 ลึก 1 |
| Button | Cylinder Preset ที่ศูนย์กลางพื้นร่อง | Radius 5, Height 2 |
| Materials | `PS_Body_Matte`, `PS_Cap_Rubber`, `PS_Button_Metal` | ด้าน / ยาง / โลหะ |

{: .note }
Cap กว้าง Ø54 ต้องเล็กกว่าหน้าแบนที่เหลือของ Body (70 − 2×6 = 58 mm) ไม่อย่างนั้นจะล้นออกไปบนขอบมน

{: .shot }
[SCREENSHOT: ภาพเรนเดอร์ Pebble Speaker บนพื้น Catcher]
