File Structure
```
Library
	Object1
		Member_1
		Member_2
	Object2
		Member_3
```

Function Keys
`F4` - แสดงเมนูเพิ่มเติม
`F12` - ย้อนกลับ
`Shift + F[numbers]` - การใช้ Function Key (`Current + 12`)

เช่น  
`Shift + F5` = `F17 `
`Shift + F10` = `F22`

Command
- `SET [LIB] [ENV]` ใช้เรียกค่า LIB ที่ได้ทำการ `EDTLIBL` จนพร้อมใช้งานแล้ว 
- `STRSQL` แล้วตามด้วย F4 ใช้ในการหาคำสั่ง 
- `EDTLIBL` ใช้ในการแก้ไข LIBRARY 
- `WRKOBJ` ใช้ค้นหา Libs และ Object และ Members 
- `CALL` เป็นการเรียกใช้ไฟล์ 

การกด F4 ระหว่างคำสั่งสามารถใช้คำหาชุด ARGRUMENT ถัดไปได้ 

ในการพัฒนาระบบของงานเราจะแบ่ง State ได้ดังนี้ 
1. `DEV`  เราจะพัฒนาระบบที่นี่ 
2. `VIT`  เราจะใช้ทดสอบระบบเรา 
3. `SIT`  เราจะทดสอบร่วมกับธนาคาร 
4. `UAT`  ธนาคารทดสอบของเขาเอง 
5. `Production`  เผยแผร่และรอ Maintain 

โดยในทีม LOANS ของเราจะใช้ 
```
SET LNS D1 
```

10/10/2023
ETP - E Touch Point
IDL