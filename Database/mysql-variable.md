# Mysql 변수 사용하기
---

프로그래머스 SQL 문제 중 입양시각구하기(2)를 풀던중 도무지 답이 뭔지 모르겠어서 구글링을 해보았다.

해당문제에서는 입양시간대에 따라 입양한 횟수를 구하는 문제였는데, 관건은 데이터에 없는 시간대까지, 즉 ```count = 0```인 시간대까지 출력해야했다.
내가 본 풀이법으로는 변수를 사용하여 풀어야한다고 한다.

## 사용법
---
#### 변수 선언법
```sql 
SET @변수이름 = 대입값;
-- or
SET @변수이름 := 대입값;
```
 - 사용할 때는 일반 변수 다루듯이 다루면 된다.
 ```sql
 SET @cnt := -1;
 select * from test_tb where num = @cnt;
 ```