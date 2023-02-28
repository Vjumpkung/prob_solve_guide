# Week 9

## หัวข้อหลัก : Dynamic Programming

### โจทย์เรียงจากง่ายไปยาก
- fin60_climb (optional) ไม่ใช่ dynamic programming
- inc
- wintsch
- elephant
- mars
- tarotora
- fin_star

### fin60_climb (optional)
- ข้อนี้คือ shortest path จากมุมซ้ายล่างไปยังมุมขวาบนใช้ Dijkstra มาประยุกต์

### inc
- แนวคิดของ dyanmic programming คือให้ for loop 2 ชั้นโดย ถ้าจำนวนที่ i มากกว่าจำนวน j ให้พิจารณา ว่าจะเอาจำนวนที่ i หรือจะเอาจำนวนที่ j แล้วบวก 1 ก็ได้ และหาค่า max ของ dp[i] และ dp[j] + 1 และพิจารณาค่า max ทุกครั้งที่ for loop จะเกิดขึ้น

### wintsch
- เป็นปัญหา weight interval scheduling ใช้ dynamic programming และ การ sort ข้อมูล โดยข้อมูลที่ให้มาจะ sort ตามเวลาจบอยู่แล้ว โดยจะ for loop 2 ชั้นโดยจะพิจารณาปัญหาย่อยคือ loop j โดยเวลาจบของ j จะต้องน้อยกว่าหรือเท่ากับ เวลาเริ่มของ i (i นำ j เสมอ) และหา maxProfit ที่ i จะต้องน้อยกว่า maxProfit ที่ j + profit ช่องที่ i

### elephant
- ช้างสามารถทำได้ 2 อย่างคือเดินหรือกระโดด เพราะว่า ช้างจะต้องวิ่ง 1 ช่องแล้วโดดขึ้นไปสูงสุดที่ 2 และลงมายังช่องที่ 3 (ปัญหานี้สามารถมองเป็น recursive ได้ หรือใช้ for loop ก็ได้)

### mars
- taps น้ำจะต้องเดาการหมุนล่วงหน้า 1 ตัวอักษรเสมอ ถึงจะได้จำนวนหยดน้ำที่น้อยที่สุด

### tarotora
- taro และ tora สามารถเลือกได้ 2 อย่างคือ ให้ taro สู้หรือ tora สู้ โดยผลต่างต้องไม่เกิน k ตัว และผลรวมต้องมีค่าน้อยที่สุด (testcase ข้อนี้มี input มากที่สุดคือ 1000)