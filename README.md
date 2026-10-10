# fist-pro in cs tu

# CS100 A2 — Responsive Learning Portfolio

หน้า A2 อยู่ที่ `index.html`; CSS ที่เขียนเพิ่มอยู่ที่ `css/style.css` และภาพเดิมยังอยู่ใน `media/` ไฟล์ A1 `main.html` และ `style.css` เก็บไว้โดยไม่แก้ไข

## ข้อมูลที่ยังต้องเติม

- วันที่ของผลงาน A1
- Reflection จากประสบการณ์จริง: What I learned, Challenge และ Next step
- รายละเอียดผลงานชิ้นที่สอง (เช่น WasteWorth หากมีข้อมูลจริง) รวม Type, Date, Role, Description, Skills, Reflection และ Evidence

## GitHub Issues ที่วางแผนไว้

ยังไม่ได้สร้าง Issues หรือ Commits จริง รายการนี้เป็นแผนให้ทำตาม workflow **Issue → Implement → Test → Commit → Close Issue**:

1. **Organize A2 project structure** — เพิ่ม `index.html`, `css/style.css` และตรวจ paths
2. **Update About Me** — เพิ่มข้อมูลนักศึกษาและรูปภาพที่มีอยู่จริง
3. **Add Portfolio Items and Evidence** — เติมผลงานอย่างน้อยสองรายการและตรวจหลักฐาน
4. **Implement Bootstrap Responsive Layout** — จัด About และ cards ให้ตอบสนองต่อขนาดหน้าจอ
5. **Test images, links, and responsive behavior** — ตรวจรูป, anchor, overflow, keyboard และ desktop/mobile
6. **Prepare GitHub Pages deployment** — ตั้งค่า Pages แล้วตรวจ URL ที่เผยแพร่จริง

## เปิดและตรวจ Responsive ใน VS Code

เปิดโฟลเดอร์โปรเจกต์ใน VS Code แล้วเปิด `index.html` ในเบราว์เซอร์ หรือใช้ส่วนขยาย Live Server หากติดตั้งไว้ จากนั้นเปิด Developer Tools ของเบราว์เซอร์ เลือกโหมดอุปกรณ์มือถือ และลองปรับความกว้างหน้าจอ ตรวจเมนู, การเรียง About, การเรียงการ์ด และการเลื่อนแนวนอน Bootstrap CSS โหลดจาก CDN จึงต้องมีอินเทอร์เน็ต

## โครงสร้างหน้าเว็บ

- Bootstrap Grid (`row`, `col-md-*`, `col-lg-6`) จัดรูปและข้อความ About เคียงกันเมื่อจอกว้าง และทำให้การ์ดแสดงสองคอลัมน์บนจอใหญ่
- `col-12` และ media query ใน CSS ทำให้การ์ดเรียงหนึ่งคอลัมน์บนมือถือ
- CSS variables ด้านบนของ stylesheet เก็บสีหลักเพื่อปรับโทนได้จากจุดเดียว
- ลิงก์ใน nav ใช้ `href="#..."` กระโดดไป section โดยไม่ใช้ JavaScript
