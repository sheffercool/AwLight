# AwLight
Bot web api AlienWorlds

1.มีฟังชั่น Auto Login (สุ่มเวลาทุกครั้งที่ Login สามารถเปิดได้ทีเดียว 30 จอ)

2.มีฟั่งชั่น Auto Mine

3.มีฟังชั่น Refresh เมื่อใช้เวลาขุดรวมนานเกิน 90 วิ(ตั้งค่าเองได้)

4.มีฟังชั่น Refresh เมื่อใช้เวลาหาค่า nonce นานเกิน 35 วิ

5.มีฟังชั่น Cpu Ram Net Mornitor ดึงค่าทุกๆ 10 วิ

6.มีฟังชั่น Use AI เมื่อ CPU มากกว่า 91 (ตั้งค่าเองได้)  ระบบ AI จะทำการตรวจค่า Cpu ทุกๆ 10 วินาที (ดึงค่าจากฟังชั่น Mornitor) หากครบ 60 ครั้ง (ครบ10นาที) แล้ว cpu ยังเกินอยู่จะขุดเลย 1 ครั้ง

7.มีฟังชั่นตรวจจับ bug ต่างๆ เช่น NaN Sec,Get time mining,Mine Too Soon ฯลฯ ทุกๆ 5 นาที

8.มีฟังชั่นAutomatic Check & Claim NFT เช็กก่อนถ้ามี nfts ถึงจะเคลม เช็คทุกๆ หลังจากขุดไป 5 ครั้ง แล้วจะเช็คก็ต่อเมื่อ Countdown to mine ครึ่งนึง จะได้ไม่ทำทรานต่อเนื่องเกินไป

9.มีฟังชั่นAutomatic Swap&Transfer เช็กก่อนถ้ามี tlm ถึง จะเช็คทุกๆ หลังจากขุดไป 5 ครั้ง แล้วจะเช็คก็ต่อเมื่อ Countdown to mine ครึ่งนึง จะได้ไม่ทำทรานต่อเนื่องเกินไป

10.พับจอได้

11.เซิฟล่มไม่ต้องกังวลเปิดคาไว้ได้ (เวลาล็อคอินจะสุ่มเวลาทำให้โอกาสล็อคอินพร้อมกันน้อยมาก) รองรับ 30-50 จอต่อเครื่อง (ขุดด้วยเครื่องตัวเอง)

12.เริ่มต้นดึงค่า เวลา และ tlm total หลังจากนั้น 10 วิถึงดึงค่า Cpu

13.รายละเอียดอื่นๆ เช่นกระเป๋า/แลนด์ ฯลฯ ต้องกดปุ่มถึงจะดึงค่า

14.เช็ค Pool ของดาวที่คุณอยู่ก่อนขุด โดยการหาค่าเฉลี่ย

15.เพิ่ม Atomic Endpoint แก้ปัญหา ติด 1020

16.เพิ่มระบบ Sleep อัตโนมัติ 4 ชั่วโมง หาก CPU ของคุณชน 100% เกิน 180 ครั้ง (ปกติ CPU จะเช็คทุกๆ 10 วิ) ข้อดีคือ คุณจะสามารถขุดได้ตลอดโดยที่ CPU ไม่เต็ม หาก Sleep บ่อย แปลว่า คุณ Stake CPU น้อยไป โดยหลังจากเทสด้วย 3 คาปา stake ที่ 110 wax ขุดแมพ x5 change time จากปกติปล่อย CPU เกิน 100 ไปเลย จะขุดได้ 0.5-0.8 TLM แต่หลังจากใช้โหมดนี้แล้ว จะขุดได้ 0.9-1.2 TLM  ซึ่งมากกว่าเดิมอย่างเห็นได้ชัด

