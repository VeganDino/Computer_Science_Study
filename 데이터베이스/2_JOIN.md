# [DB] JOIN

### 조인이란?

두 개 이상의 테이블이나 데이터베이스를 연결하여 데이터를 검색하는 방법      
테이블을 연결하려면, 적어도 하나의 컬럼을 서로 공유하고 있어야 하므로 이를 이용하여 데이터 검색에 활용한다.         

<br>

### JOIN 종류

-INNER JOIN     
-LEFT OUTER JOIN        
-RIGHT OUTER JOIN       
-FULL OUTER JOIN        
-CROSS JOIN     
-SELF JOIN      

<br>

### INNER JOIN  

교집합. 기준 테이블과 join 테이블의 중복된 값을 보여준다.   

<img src ='https://user-images.githubusercontent.com/56749776/136809249-6f9394fc-d0a7-4b81-bdda-e4f91632241e.png' width='60%'>

```SQL
SELECT A.NAME, B.AGE FROM A
INNER JOIN B ON A.EMP = B.EMP
```

<br>

### LEFT OYTER JOIN

기준 테이블값과 조인 테이블과 중복된 값을 보여준다.     
왼쪽 테이블 기준으로 JOIN 한다고 생각하면 됨.

<img src ='https://user-images.githubusercontent.com/56749776/137591878-aa86a1a0-d63a-4263-9185-869d12fe4da6.png' width='60%'>

```SQL
SELECT A.NAME, B.AGE FROM A
LEFT OUTER JOIN B ON A.EMP = B.EMP
```