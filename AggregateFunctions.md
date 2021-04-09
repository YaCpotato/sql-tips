## Aggregate Functions
### boolean COUNT
#### SQL
```sql
select
  count(bool) as bool_cnt
  ,count(*) as row_cnt
from
  values
    (1, true)
    ,(2, false)
    ,(3, true)
  as t (id,bool)
```

#### OUTPUT
|bool_cnt|row_cnt|
|:--:|:--:|
|2|3|
