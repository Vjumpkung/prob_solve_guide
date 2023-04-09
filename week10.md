# Week 10

## หัวข้อหลัก : Dynamic Programming

### โจทย์เรียงจากง่ายไปยาก
- lcs1
- lcs2
- seqalign
- rna
- cutting stick
- supersale

### lcs1 & lcs2
- ใช้ recurrence ที่เรียนจากวิชา algorithm มาทำการแก้โจทย์ได้เลย 

### seqalign
- ใช้ recurrence ที่เรียนจากวิชา algorithm มาทำการแก้โจทย์ได้เลย

### rna
- ใช้ recurrence ที่เรียนจากวิชา algorithm มาทำการแก้โจทย์ได้เลย

### NOTES สำหรับ 3 ข้อแรก
- https://gitlab.com/jittat/01204313-algorithms-65/-/blob/main/lectures/algo-65-12-dp-2-2023-03-1.pdf

### cutting stick
- recurrence คือ 
- `dp(l,r) = min(for i in range(l,r) : dp(l,i) + dp(i,r) + cost[r] - cost[l])`

### supersale
- 2d dynamic programming
- https://www.geeksforgeeks.org/0-1-knapsack-problem-dp-10/
