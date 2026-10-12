---
title: "🤔 SketchUp ทำได้ไหม? 10 ข้อ"
nav_order: 83
permalink: /can-sketchup/
---

# SketchUp ทำได้ไหม? 10 อย่างที่ formZ ทำได้ในคลิกเดียว
{: .no_toc }

SketchUp ใช้ง่ายและดีมาก **แต่มีหลายอย่างที่ต้องลง extension** หน้านี้รวม 10 อย่างที่ formZ ทำได้ในตัว แต่ละการ์ดใช้เวลาไม่เกิน 1 นาที และมีลิงก์ไปบทที่สอน **เราตั้งใจเทียบอย่างยุติธรรม** ข้อไหนที่เสมอกันก็บอกว่าเสมอ

{: .shot }
[SCREENSHOT/CLIP: คลิป 30–60 วินาทีต่อการ์ด (อัด screen ใน formZ) วางบนการ์ดแต่ละใบ]

{% for c in site.data.can_sketchup %}
### {{ c.id }}. {{ c.title }}
{: .no_toc }
<div class="can-su">
<p class="mb-1">🟣 <strong>formZ:</strong> {{ c.fz }} · 🏠 ลองกับ: {{ c.obj }}</p>
<p class="mb-1">⚪ <strong>SketchUp:</strong> {{ c.su }}</p>
<p class="mb-0">ผล: <strong>{{ c.verdict }}</strong> · <a href="{{ c.ch | relative_url }}">▶ ไปบทที่สอน</a></p>
</div>
{% endfor %}

{: .verify }
ข้อมูลฝั่ง SketchUp อ้างอิง SketchUp Pro 2026 (เช่น Solid Tools มีเฉพาะ Pro) และคลิปยอดนิยมของช่อง SketchUp ทางการ เช่น "Rounded Cube with Native Tools" (7:50 นาที) ควรตรวจกับ Help Center ล่าสุดก่อนนำไปสอน: https://help.sketchup.com/

{: .note }
อยากเห็นว่าทำง่ายแค่ไหน? ลอง [C0 บท 3: กล่องมุมมนใน 60 วินาที]({{ '/courses/c0-start-here/03-rounded-box/' | relative_url }})
