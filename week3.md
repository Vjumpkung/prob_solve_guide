# Week 2

## หัวข้อหลัก : Graph

### โจทย์เรียงจากง่ายไปยาก
- robot2000 
- robot1000s (optional)
- ku01_under
- mid59_mask
- conncount
- box
- qualitymap
- jumppoint
- lemmo (optional) (ยังไม่ผ่านทุก testcases)

### robot2000
- เป็นการแปลภาษาจาก robot1000 ให้เป็น robot2000

### robot1000s (optional)
- ใช้การบวกลบเลขเพื่อหาจุดที่ robot ไปไกลที่สุด

### ku01_under
- พิจารณาจุดที่สามารถลอดได้ทั้งหมด (บวกทีละ 0.5 ได้)

### mid59_mask
- ให้เก็บ index จาก 1 ไว้ที่ตัวเลขที่รับมาจะคำนวณง่ายขึ้น

### conncount
- ใช้ union find หรือ dfs,bfs จาก vertex ที่ดีกรีสูงสุดก่อน

### box
- ใช้ DFS จะง่ายกว่า BFS เพราะว่าสนใจแค่ว่าเดินทางไปถึงได้หรือไม่เท่านั้น

### qualitymap
- ใช้ DFS โดยตะค่อยๆพิจารณาจุดที่เป็น $ หรือ * และใช้ตัวแปรเป็น global เพื่อความสะดวก

### jumppoint
- เป็น BFS โดยสร้าง Graph จากเงื่อนไขที่โจทย์กำหนด

### lemmo (optional) (ยังไม่ผ่านทุก testcases)
- ไม่แน่ใจเรื่องวิธีทำที่ผ่านแต่เดินตรงๆ ตามโจทย์จะไม่ทัน 1 วินาที