---
Start Date: 2023-10-10
---
## เนื้อหาประจำวันที่ 10/10/2023

ค้นหา Object ว่าอะไรบ้าง
```
WRKOBJ
```

จัดการ Library
```
EDTLIBL
```

ค้นหาข้อมูล
```
WRKQRY
```

เช็ค Spool file
```
WRKSPLF
```

เขียน Query SQL
```
STRSQL
```

คัดลอกไฟล์
```
CPYF
```

Work with Object using DPM
```
WRKOBJPDM
```

เปิด Programming 
```
STRPDM
```

ดูรายละเอียดตาราง
```
DSPFD
```

ดูรายระเอียดตาราง - Silverlake Only
```
DSPFF
```

ดูรายระเอียดตาราง - IBM
```
DSPFFD
```


สำหรับ Attribute ในไฟล์ Record
PM = Physical File - ไฟล์ที่เอาไว้เก็บข้อมูล
LM = Logical File - ไฟล์ที่เอาไว้ดึงข้อมูลจากไฟล์หลักมาเขียน Logical เพิ่มเติมเช่น การเรียง

การใช้ `WRKQRY`
- Specify file selections เลือกไฟล์ที่จะดึงข้อมูล
- Define result fields - เอาไว้ดำเนินการเพิ่มเติม
- Select and sequence fields - เลือกไฟล์ที่จะแสดงผล และลำดับ
- Select records - เหมือน `WHERE` ใน `SQL`
- Select sort fields - เลือกเรียงมากไปน้อยหรือน้อยไปมาก และเลือกความสำคัญ
- Select report summary functions เลือกข้อมูลที่เป็นตัวเลขมาดำเนินการ `Total`, `Average`, `Minimum`, `Maximum`, `Count`
- Define report breaks เอาไว้แบ่งผลออกจากกันเพื่อความง่ายในการอ่าน ส่วนมากใช้คู่กับ `Select report summary functions`
