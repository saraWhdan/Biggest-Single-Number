# Biggest-Single-Number




Problem Link:https://leetcode.com/problems/biggest-single-number/description/?envType=study-plan-v2&envId=top-sql-50

## Solution
```sql
select MAX(num) num from
(select num 
from MyNumbers
group by num
having count(*)=1) t
