# learn-formz

เว็บสอน formZ 10 + RenderZone ภาษาไทย (Jekyll + Just the Docs) สำหรับ GitHub Pages

## รันบนเครื่อง
```bash
bundle install
bundle exec jekyll serve
# เปิด http://127.0.0.1:4000/learn-formz/
```

## โครงสร้าง
- `index.md` แคตตาล็อก course
- `courses/<course>/index.md` หน้า course (parent) และ `courses/<course>/NN-*.md` บทเรียน (`chapter: true` → มีปุ่มก่อนหน้า/ถัดไปอัตโนมัติ)
- `glossary.md` อภิธานศัพท์กลาง · `references.md` แหล่งอ้างอิง
- `_includes/meta.html` (เวลาอ่านและเวลาลงมือ), `_includes/homework.html` (กล่องการบ้าน Phase 1: localStorage), `_includes/footer_custom.html` (prev/next)
- `assets/images/<course>/` ใส่ภาพ screenshot ตาม placeholder `[SCREENSHOT: ...]`
- `.github/workflows/pages.yml` build และ deploy ไป GitHub Pages (Settings > Pages > Source: GitHub Actions)

## Callouts
`{: .easy }` ง่ายเหมือน SketchUp · `{: .power }` SketchUp ทำไม่ได้ · `{: .shapr }` Shapr3D→formZ · `{: .verify }` ต้องยืนยัน · `{: .shot }` screenshot · `{: .warning }` · `{: .note }`
