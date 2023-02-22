# Week 4 
## หัวข้อหลัก Greedy , Graph Search

### โจทย์เรียงจากง่ายไปยาก
- intsch (greedy interval scheduling)
- maxlate (greedy maximum lateness)
- mid592_maze (optional) (ใช้ DFS) **OPTIONAL**
- topo (topo ตรงๆ)
- uva10305_orderingtasks (topo ประยุกต์นิดหน่อย)
- bipartite (ตรงๆ เลย)
- mid62_ttt (bipartite ประยุกต์)
- twoteams (bipartite ประยุกต์) **OPTIONAL**
- mid64_shipmentcost (BFS แบบประยุกต์หน่อย) 
- mid61_dig (brute force possible) **OPTIONAL**
- fin_toofast (Shortest Path 2 มิติ)
- mid64_redblackbridges (Shortest Path 3 สี) **OPTIONAL**
- stardrawing (DFS) **OPTIONAL**

### intsch (Interval Scheduling)
- แนวทางการทำคือ ให้ sort ก่อนแล้วเลือก earliest finish time ที่เร็วที่สุด แล้วเอาไปเปรียบเทียบกับ start time ของ interval ต่อไป

### maxlate (Maximum Lateness)
- แนวทางการทำคือ ให้ sort ก่อนแล้วพิจารณาเวลาที่ late **มากที่สุด**

### mid592_maze (optional)
- ข้อนี้จะคล้ายๆ Maze แต่เราจะต้องเขียน DFS ให้เร็วๆ โดยการเก็บ visited ใน array 2 มิติ และเก็บค่าที่เคยเจอไว้ใน array 2 มิติ โดยที่ array 2 มิตินี้จะเก็บค่าที่เคยเจอไว้ในรูปของ ค่าที่เคยเจอ และ จำนวนของค่าที่เคยเจอ

### topo (Topological Sort)
- โจทย์ข้อนี้จะใช้เรื่อง Topological Sort โดยจะเลือก node ที่มี indegree เป็น 0 แล้วลบ edge ออก แล้วทำซ้ำจนกว่าจะเหลือ node ที่มี indegree เป็น 0 แล้วเราจะได้ answer ที่เรียงตาม Topological Sort แต่ถ้าเจอ cycle แสดงว่าจะหา answer ไม่ได้

### uva10305_orderingtasks (Topological Sort)
- โจทย์ข้อนี้จะให้เราเรียง task ตาม Topological Sort แต่จะมีเงื่อนไขว่า ถ้ามีหลาย task ที่มี indegree เป็น 0 ให้เราเลือก task ที่มี id น้อยกว่าก่อน

### bipartite
- โจทย์ข้อนี้ให้พิจารณากราฟโดยตรวจสอบว่าเป็น Bipartite มั้ย ซึ่งใช้ BFS ในการแบ่งกราฟออกเป็น 2 กลุ่มได้

### mid62_ttt
- โจทย์ข้อนี้เป็นการนำเรื่อง bipartite มาประยุกต์เข้าด้วยกัน โดยตัด edge ตามโจทย์ แล้วเราจะได้กราฟที่เป็น Bipartite แล้วเราจะต้องหาว่าจะเลือกจุดที่เป็น 1 ในกราฟที่เป็น Bipartite ที่มีจำนวนมากที่สุด โดยจะใช้ BFS ในการหาจำนวน 1 ในกราฟที่เป็น Bipartite

### twoteams (optional)
- ไม่แน่ใจเรื่องวิธีทำ (ใช้ Binary Search + BFS + Bipartite Check)

### mid64_shipmentcost
- key หลักของข้อนี้คือถ้าอยากพิจารณา BFS โดยถ้าอยากได้ layer หลายๆ layer ให้เอา node ที่ต้องการใส่เข้าไปใน queue ล่วงหน้าก่อนเลย

### mid61_dig (optional)
- ข้อนี้จะคล้ายๆกับ mid592_maze (optional) โดยสามารถเจาะรูทีละรูเพื่อใช้ในการเดินทางไปยังจุดหมายได้ โดยจะใช้ BFS เพื่อหาระยะทางที่สั้นที่สุด

### fin_toofast (Shortest Path 2 มิติ)
- ข้อนี้ควรทำโจทย์ข้อ Shortest Path ก่อนเพราะว่ามีการใช้ Dijkstra Algorithm ในการหา shortest path และมีกรณีพิเศษในการเดินทาง

### mid64_redblackbridges (Shortest Path 3 สี) (optional)
- ข้อ red black bridges ใช้เรื่องของ BFS แต่จะต้องแยก visited, layer ของ bfs ออกเป็น 3 มิติเพื่อพิจารณาการเดินให้ครบทุกกรณี

### stardrawing (optional)
- ข้อนี้ **ยากมาก!!!!!!!!** ใช้ DFS โดยจะพิจารณา node ที่มี degree 3 ก่อนแล้วพิจารณาว่ามี cycle มั้ย (อย่าหาทำ)
