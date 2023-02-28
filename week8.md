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

### probe1d (โจทย์ใช้ Lib)
- โจทย์ปิดไปแล้ว
- ใช้ binary search

### traffic (โจทย์ใช้ Lib)
- ให้ linear search ก่อนแล้วค่อย binary search

### inversion
- ใช้ merge sort แล้วนับจำนวน inversion

### ioi_maintain (Minimum Spanning Tree)
- แนะนำให้ใช้ kruskal เพราะว่าเร็วกว่ามากๆ และควรจะทำให้ Minimum spanning tree จบภายใน O(n) n หมายถึงจำนวน node