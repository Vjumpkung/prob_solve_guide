# Week 2

## หัวข้อหลัก : linked-list

### โจทย์เรียงจากง่ายไปยาก
- listwork 1 ( Linked List Practice 1 )
- listwork 2 ( Linked List Practice 2 )
- ic
- trains
- throwingcards1
- broken (must use text file to run program)
- rails
- ku01_distinct (solution must be O(n^2))
- ku01_cars (optional) (solution must be O(n))
- necklace (union set disjoint is alternative solution)
- chains (optional) ยากสุดกำลัง

### listwork 1 ( Linked List Practice 1 )
- เป็นโจทย์ที่จะให้ลองใช้ STL list และ iterator ในการทำงาน

### listwork 2 ( Linked List Practice 2 )
- เป็นโจทย์ที่จะให้ลองใช้ STL list และ iterator ในการทำงาน

### ic
- ข้อนี้ให้ระวังเรื่องการหมุนซ้ายหรือขวาโดย list ไม่มีสมาชิกอะไรอยู่เลย (empty)

### trains
- ใช้ splice จะเร็วกว่า insert และควรประกาศ array of list ไว้ที่ 100000 เลยใน global variable

### throwingcards1
- อ่านเงื่อนไขตามโจทย์และใช้ vector เพื่อเก็บค่าที่โยนไพ่ได้

### broken
- ปุ่ม Home หมายถึงเลื่อน cursor การพิมพ์ไปข้างหน้าสุด และ End หมายถึงเลื่อน cursor การพิมพ์ไปข้างหลังสุด 

### rails
- เป็นโจทย์ที่ใช้เรื่อง stack โดยเป็นการถามคำถามว่า ลำดับของรถไฟสามารถ เข้า และ ออกเป็นลำดับที่ถูกต้องได้หรือไม่

### ku01_distinct
- เป็นโจทย์ที่จะให้ลองใช้ STL set โดยให้เก็บค่าที่เข้ามาเป็น set และใช้ size() เพื่อนับจำนวนค่าที่เข้ามา

### ku01_cars (optional)
- ให้ลอง loop ถอยหลังดูแล้วจะเห็นอะไรบางอย่างได้

### necklace
- ข้อนี้ไม่จำเป็นต้องเขียน linked list เอง สามารถใช้ STL list ได้แต่ต้องใช้ algorithm ดีๆ

### chains (optional)
- **ข้อนี้ยากสุดๆ** ทุกๆคำสั่งควรทำจบใน O(1) และเวลาเฉลี่ยของโปรแกรมควรเป็น O(n) หมายถึงรับ input แล้วเวลาการทำงานไม่เกิน 0.5 วินาที