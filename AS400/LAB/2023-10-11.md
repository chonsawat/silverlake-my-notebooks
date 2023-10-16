## เนื้อหาประจำวันที่ 11/10/2023

เปิด ALDON
```
SRTLMI
```
- ฝ่ายเราใช้ `LNS*`
- Release / Application / Group
	- ตัวอย่าง `BASE/LNS/SIBS`

- Silverlake
	- `LN [ประเภท] [การดำเนินการ] [3 ตัวหลังเลขที่ยังว่าง]`
	- ม็อบให้ใช้ 96998

- ประเภท
	- 8 - รายการ
	- 9 - พารามิเตอร์

* Inqeury - การดำเนินการ
	* 5 - ดูทุกรายการ
	* 6 - ดูแต่ละรายการ
	* 7 - เพิ่มข้อมูล
	* 8 - แก้ไขข้อมูล
	* 9 - ลบข้อมูล

* งานเรา
	* Service สื่อสารไปที่ Service เพื่อไปคุม Application
	* Program ไปคุยกับ Service (แต่โปรแกรม ต้องมี Module เสมอ)
	* Module เอาไว้เก็บโปรแกรม

```
CLM หลักประกันและ แฟ้มวงเงิน (Facility)
LNS เงินกู้
```

```
QLNSMBHRLE
QLNSMBHDDS
QLNSSRCDDS

Q - พวกโค๊ด
LNS - Loans
MBH - M Base Handler

DDS - Data file
RLE - RPGLE
```


Program attribute
- BND - Binary Program
- ILE - ใช้บ่อยๆ
- OPM

- Service
- Prpgram
- module
- input
- reponse

Parameter - เหมือนตัวอธิบาย Argument แต่ละตัว
Day Mode - อยู่ตลอดการทำงาน
Work file - ไฟลที่จะพักไว้เอาจาก Database

![[Pasted image 20231011104944.png]]
![[Pasted image 20231011105009.png]]


# Specification

- [ ] F - [[File Description Specification]]
- [ ] D - Definition Specification
- [ ] C - Calculation Specification
- [ ] H - Control (Header) Spectification ใช้กับ Binary file ส่วนมากพวกเทพจะเขียน
- [ ] I - Input Specification
- [ ] O - Output report

- [ ] `I` - Insert
- [ ] `I[number]` - Insert Multiple Line
- [ ] `D` - Delete
- [ ] `DD` - Delete to `DD`
- [ ] `C` - Copy using with `A` or `B`
- [ ] `CC` - Copy multiple line using with `A` or `B`
- [ ] `M` - Move using with `A` or `B`
- [ ] `MM` - Move multiple line using with `A` or `B`
- [ ] `A` - Paste Copy after A
- [ ] `B` - Paste Copy before B

--- บ่าย ---
REF - ดึง Data Dictionary มาใช้

Record Name จะตั้งชื่อเหมือนไฟล์ที่กำลังทำ

ACC - 19
Code - 10
Money - 17, 2
ดอกเบี้ย - 19, 5
Percentage - 11, 9

Data Type
-BLANK- - จะ Pack เป็น Decimal
S - Zone เลขจำนวนเต็ม
A - เป็น Character


# RPG Command
`FILE` in brows
`SAVE` in brows
`CAN`


14 - Compile

`enironment`
![[Pasted image 20231011140418.png]]

![[Pasted image 20231011140749.png]]

Error
![[Pasted image 20231011141118.png]]

ALDON ใช้ดู Spool File

**Function**
COLHDG - กำหนดชื่อ Field
TEXT - ส่วนมากใช้ตอนออก Report
REF - Ref มาได้แค่ไฟล์เดียว
REFFLD - 

---

REF, REFFLD

![[Pasted image 20231011152510.png]]
![[Pasted image 20231011151944.png]]

---

Dependency Object

![[Pasted image 20231011151902.png]]

___

LN96135
LN3818C

___

File Type
- `I` - อ่านข้อมูล
- `O` - 
- `U`

File Addition
- `BLANK`
- `A` - เพิ่มข้อมูลได้

___

# Conclusion
```
 Columns . . . :    1 108                                      Browse                                         STHDVLNSAL/QLNSSRCDDS 
 SEU==>                                                                                                                    LNTEST02 
 FMT PF .....A..........T.Name++++++RLen++TDpB......Functions+++++++++++++++++++++++++++ ...+... 9 ...+... 0 ...+...                
        *************** Beginning of data ***************************************************************************************   
0001.00                                             REF(LNMAST)                                                          231011     
0002.00                 R RLNTEST02                                                                                      231012     
0003.00      A            LNNO           5S 0       COLHDG('LOANS NO ACCOUNT')                                           231011     
0004.00      A            LNNAME        10A         TEXT('NAME OF ACCOUNT')                                              231011     
0005.00      A            LNADDR       200A                                                                              231011     
0006.00      A            LNLNS         19S 0                                                                            231011     
0007.00      A            PRATE         19S 0                                                                            231011     
0008.00      A            LNSOM        200A                                                                              231011     
0009.00      A            ACCTN     R               REFFLD(ACCTNO)                                                       231011     
0010.00                   TYPE      R                                                                                    231011     
0011.00                   LNPWF     R               REFFLD(LNPWFC LNPRWC)                                                231011     
0012.00                   LNPWFC    R               REFFLD(LNPWFC LNPRWC)                                                231011     
0013.00                                                                                                                  231011     
        ****************** End of data ******************************************************************************************   
                                                                                                                                    
```