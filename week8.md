# Week 8

## หัวข้อหลัก : Minimum Spanning Tree , Divide and Conquer

### โจทย์เรียงจากง่ายไปยาก
- uva11462_agesort_merge (ใช้ std::sort ผ่าน)
- probe1d (โจทย์ใช้ Lib)
- traffic (โจทย์ใช้ Lib)
- inversion
- ioi_maintain (Minimum Spanning Tree)

### uva11462_agesort_merge (ใช้ std::sort ผ่าน)
- ใช้ merge sort ที่เขียนเองก็ได้หรือใช้ sort จาก `#include <algorithm>` ก็ได้

### probe1d (โจทย์ใช้ Library)
- โจทย์ปิดไปแล้ว
- ใช้ binary search

### traffic (โจทย์ใช้ Library)
- ให้ linear search ก่อนแล้วค่อย binary search

### inversion
- ใช้ merge sort แล้วนับจำนวน inversion

### ioi_maintain (Minimum Spanning Tree)
- แนะนำให้ใช้ kruskal เพราะว่าเร็วกว่ามากๆ และควรจะทำให้ Minimum spanning tree จบภายใน O(nlogn)
- นิยามของ Minimum Spanning Tree คือมี n - 1 edges ที่มีน้ำหนักรวมทั้งหมดน้อยที่สุด ดังนั้นเมื่อ union ครบ n - 1 รอบแล้วให้หยุดหา minimum spanning tree ทันทีเพราะไม่มี edge ที่น้อยกว่า edge ที่มีอยู่แล้ว