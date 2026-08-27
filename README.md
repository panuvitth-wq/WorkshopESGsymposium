# Workshop ESG Symposium 2026 — Track 3: Climate Adaptation

Interactive workshop board สำหรับ **SCG Internal Sharing Session** (2 September 2026)
หัวข้อ *Business Water Resilience*

**Live:** https://panuvitth-wq.github.io/WorkshopESGsymposium/

---

## เนื้อหา

| แท็บ | รายละเอียด |
|---|---|
| 1️⃣ สิ่งที่ธุรกิจต้องทำ | ภาคธุรกิจควรเตรียมตัวและรับมืออย่างไรกับสถานการณ์น้ำท่วมและภัยแล้งที่รุนแรงมากขึ้น? → หมวด **A. Risk Assessment / B. Vulnerability Management / C. Monitoring & Warning System** |
| 2️⃣ ข้อเสนอแนะภาครัฐ | ข้อเสนอแนะที่อยากให้ภาครัฐบาล/หน่วยงานที่เกี่ยวข้องสนับสนุน → 4 มิติ **Policy / Community / Data / Infrastructure** |
| 📊 Dashboard | รวมผลทั้ง 2 คำถามในหน้าเดียว — สถิติ, สัดส่วนแต่ละหมวด, บอร์ดโพสต์อิท, ค้นหา, ย้ายหมวด, Export CSV |

ไฟล์เดียวจบ ไม่มี build step ไม่มี dependency (โหลดเฉพาะฟอนต์ Sarabun จาก Google Fonts)

---

## วิธี deploy บน GitHub Pages

1. อัปโหลดไฟล์ในโฟลเดอร์นี้ (`index.html`, `.nojekyll`, `README.md`) ไปที่ root ของ repo
   `panuvitth-wq/WorkshopESGsymposium` บน branch `main`

   ```bash
   git clone https://github.com/panuvitth-wq/WorkshopESGsymposium.git
   cd WorkshopESGsymposium
   cp /path/to/gh-pages/* .
   cp /path/to/gh-pages/.nojekyll .
   git add -A && git commit -m "Add Climate Adaptation workshop board" && git push
   ```

   หรือใช้เว็บ: **Add file → Upload files** แล้ว Commit

2. ไปที่ **Settings → Pages**
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` / โฟลเดอร์ `/ (root)` → **Save**

3. รอ 1–2 นาที เว็บจะขึ้นที่
   `https://panuvitth-wq.github.io/WorkshopESGsymposium/`

4. สร้าง QR Code จาก URL ข้างต้นไปใส่ในสไลด์/ป้ายในห้องประชุม

---

## ข้อควรทราบเรื่องข้อมูล

ข้อมูลถูกเก็บด้วย **localStorage ของเบราว์เซอร์แต่ละเครื่อง** — คำตอบจะไม่ถูกส่งขึ้น server
(เหมาะกับกรณีผู้ดำเนินรายการเป็นคนพิมพ์รวมจากเครื่องเดียว หรือฉาย Dashboard จากเครื่องหน้าห้อง)

หากผู้เข้าร่วมสแกน QR แล้วกรอกจากมือถือของตัวเอง **แต่ละคนจะเห็นเฉพาะคำตอบของตัวเอง**
ถ้าต้องการรวมคำตอบจากทุกเครื่องมาที่ Dashboard เดียว ต้องต่อ backend เพิ่ม
(เช่น Google Apps Script + Google Sheet, Firebase Firestore หรือ Supabase)

- ปุ่ม **Export CSV** ใช้เก็บผลหลังจบ session
- ปุ่ม **ใส่ข้อมูลตัวอย่าง** ใช้ทดสอบหน้าตา Dashboard ก่อนงานจริง
- ปุ่ม **ล้างข้อมูลทั้งหมด** ใช้เคลียร์ก่อนเริ่ม session จริง

---

*Internal Use Only — For SCG Employees*
