## 3. Function name : MaxLoanAmount
**Input** : `amount`

**Step** :

1. คำนวณมูลค่าเงินโดยเรียกใช้ `sumLoanAmount` โดยจะรวมมูลค่าจากนั้นนำไปคูณกับ 0.95
2. เรียกใช้ `checkCreditLimit` เพื่อเช็คว่าถ้ากู้เกิน 10 ล้านจะได้แค่ 10 ล้าน

**Output** : `amount`

| **Input**  | **Example**  |
| -------------|:------------|
| amount | 5000 |

| **Output**  | **Example**  |
| -------------|:------------|
| amount | 4750 |