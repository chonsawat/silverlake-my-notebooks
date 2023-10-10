![[Pasted image 20231010085728.png]]

# Corporate information
Aldon คือหน่วยทางธุรกิจที่ใช้ในการพัฒนาและสนันสนุนโปรแกรมในการเปลี่ยนสินค้าสำหรับ enterprise แอพพลิเคชัน
- Application life cycle management (ALM)
- Software change management (SCM)

Rocket Software, Inc พัฒนาสินค้า infrastructure สำหรับ 4 อย่างนี้เป็นหลัก
- Storage, Networks, and Compliance
- Database server and tools
- Business information and analytics
- Application development, integration, and modernization

Rocker Aldon Lifecycle Manager ( `IBM i Edition` หรือ `LM(i)` )
ช่วยในการจัดเตรียมและ automated method สำหรับการปรับปรุงตลอดทั้งกระบวนการดำเนินงาน

(ข้ามหน้า 6 ประวัติ)

# What does LM(i) help?
- `LM (i)` เครื่องมือในการจัดการการเปลี่ยนแปลงที่จัดเตรียม Methods ที่ใช้ในการ Maintain ไว้ให้โดยอัตโนมัติตลอดทั้งกระบวนการดำเนินการ
- ซอฟแวร์ในการจัดการการเปลี่ยนแปลงและจัดการแหล่งที่มาสำหรับ enterprise application lifecycle
- ด้วย `LM (i)` โปรแกรมมือจะต้อง "check out" สำเนาของ Object เพื่อเปลี่ยนมัน
- `LM (i) logs` แสดงประวัติการ checkout และทำให้แน่ว่าจะไม่มีใคร check out โดยไม่ได้ตั้งใจในโปรแกรมเดียวกัน เมื่อเปลี่ยนแปลงสำเร็จ โปรแกรมเมอร์เรียกหาหรือทำการเลื่อนตำแหน่งไปที่ `enivronment` สำหรับใช้ทดสอบ
- เมื่อ `Object` 

-- จากหน้า 8 
(โดดข้ามไปอ่านหน้า 13 ก่อน)

# Basic Terms and Concept

**Group**
Aldon LM(i) `Group` หรือ `Application group` เป็นชื่อของ `category` ที่ทำให้เราจัดการ `Application group` กันได้ง่ายขึ้น

**Application**
ด้วย `Aldon LM(i)` ตัว `Object` ที่เกี่ยวข้องจะนิยามว่าเป็น `Application`

**Release**
เกี่ยวกับกลุ่มของ `libraries` ที่รวบรวม `objects` ที่ถูกใช้สร้าง `Application`

![[Pasted image 20231010100024.png]]

Something