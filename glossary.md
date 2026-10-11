---
title: "อภิธานศัพท์ (Glossary)"
nav_order: 90
permalink: /glossary/
---

# อภิธานศัพท์ (Glossary)

ศัพท์ทุกคำใช้ **ชื่อภาษาอังกฤษตามเมนู official ของ formZ 10** เพื่อให้ตรงกับที่เห็นบนหน้าจอ ตามด้วยคำอธิบายภาษาไทย
คอลัมน์ "บท" บอกว่าพบคำนี้ครั้งแรกในบทไหน

{% assign terms = site.data.glossary | sort_natural: "term" %}
<table>
<thead><tr><th>English term</th><th>คำอธิบายภาษาไทย</th><th>บท</th></tr></thead>
<tbody>
{% for t in terms %}<tr id="{{ t.term | slugify }}"><td><strong>{{ t.term }}</strong></td><td>{{ t.th }}</td><td>{{ t.ch }}</td></tr>
{% endfor %}
</tbody>
</table>

<small>มีทั้งหมด {{ terms.size }} คำ และจะเพิ่มตาม course ที่เขียนใหม่ (แก้ได้ที่ `_data/glossary.json`)</small>
