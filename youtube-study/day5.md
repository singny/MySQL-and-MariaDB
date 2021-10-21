# day5
## 1. INNER JOIN
### - 키 값이 있는 테이블의 컬럼 값을 비교 후 조건에 맞는 값만 가져오는 것이다.
![image](https://user-images.githubusercontent.com/89372116/138336726-5cf4447e-309e-469b-bea8-564d64c41e37.png)
```
SELECT * FROM A테이블 INNER JOIN B테이블 ON A테이블.a컬럼 = B테이블.b컬럼;
```
![image](https://user-images.githubusercontent.com/89372116/138337415-8ce1a02a-c6cc-44e4-929d-0431675afea5.png)
## 2. CROSS JOIN 
### - 조인되는 두 테이블에서 곱집합을 반환한다.
### - 테이블의 각 값을 연결하여 테이블 행의 수를 모두 곱한 값만큼 만들어진다.
![image](https://user-images.githubusercontent.com/89372116/138337705-4fdec3ae-56ad-4203-98ca-d59e0aa6562f.png)
```
SELECT * FROM A테이블 CROSS JOIN B테이블;
```
![image](https://user-images.githubusercontent.com/89372116/138337952-932e2f62-59af-43c6-9615-42f127a89d99.png)
## 3. OUTER JOIN
### 3-1. LEFT OUTER JOIN 
#### - LEFT OUTER JOIN은 조인문의 왼쪽에 있는 테이블의 모든 결과를 가져온 후 오른쪽 테이블의 데이터를 매칭하고, 매칭되는 데이터가 없는 경우 NULL을 표시한다.
![image](https://user-images.githubusercontent.com/89372116/138338862-b2efd8f1-7029-47da-99de-a2f3d5ece9a8.png)

```
SELECT * FROM A테이블 LEFT OUTER JOIN B테이블 ON A.a컬럼 = B.b컬럼;
```
![image](https://user-images.githubusercontent.com/89372116/138338781-89a2c280-1c53-4f83-b37c-63281292224c.png)
### 3-2. RIGHT OUTER JOIN
#### - RIGHT OUTER JOIN은 조인문의 오른쪽에 있는 테이블의 모든 결과를 가져온 후 왼쪽의 테이블의 데이터를 매칭하고, 매칭되는 데이터가 없는 경우 NULL을 표시한다.
![image](https://user-images.githubusercontent.com/89372116/138339000-d6d7ee8a-9344-4eb4-83b5-a7b2c6cafb7f.png)
```
SELECT * FROM A테이블 RIGHT OUTER JOIN B테이블 ON A.a컬럼 = B.b컬럼;
```
### 3-3. FULL OUTER JOIN
#### - Full Outer Join은 LEFT OUTER JOIN과 RIGHT OUTER JOIN을 합친 것이다. 양쪽 모두 조건이 일치하지 않는 것들까지 모두 결합하여 출력한다.
![image](https://user-images.githubusercontent.com/89372116/138339310-6037fa70-211a-4dd9-a843-2418c08d760a.png)
## 4. NATURAL JOIN
### - 공통된 속성을 찾아 같은 값을 갖는 항목끼리 결합시켜준다.
![image](https://user-images.githubusercontent.com/89372116/138340257-a2707e4b-9c6e-49bd-b32c-826425c579f9.png)
```
SELECT * FROM A테이블 NATURAL JOIN B테이블;
```
## * 칼럼 이름 변경하기
```
SELECT A테이블.a칼럼 AS 변경하고 싶은 칼럼명 FROM A테이블 LEFT(RIGHT) JOIN B테이블 ON A테이블.a칼럼 = B테이블.b칼럼;
```
![image](https://user-images.githubusercontent.com/89372116/138341183-873284ed-0f5b-4d4e-9483-0757d1d7b48b.png)

