## Tuple 튜플
### Tuple 특징

- 시퀀스 자료형
- 수정, 추가, 삭제가 불가능한 리스트 - 읽기 전용
- 왜 쓸까?
    - 메모리 사용이 효율적
    - 읽기만 가능하기 때문에 데이터 손실 염려가 없다

### Tuple 만들기

- List는 대괄호 [] 이지만 튜플은 소괄호이며, 괄호 생략이 가능하다
- `튜플 = (데이터, 데이터, 데이터)`
- `튜플 = 데이터, 데이터, 데이터`
- 소괄호 : 함수에서 사용
- 대괄호 : List를 정의할 때
- 중괄호 : f-string에 사용, 딕셔너리
- 예시
    
    ```python
    # 튜플 만들기
    1.  a = (3, 4, 5)
    		a = "문자열", 3, True
    2.  a = (30,) # 한개를 만들 때에는 뒤에 콤마를 붙여야 한다.
    		a = 30,   # 생략시에도 같음
    
    # 튜플을 리스트로 만들기
    1. a = tuple([5,6,7])  # 리스트를 tuple()로 감싸면 된다. 자료형 변환이 일어남 (5,6,7)로 바뀌게 됨
    2. x = list(range(10)) # range객체를 list감싸면 list 자료형이 된다. [0,1,2,...,9]
       a = tuple(x)        # tuple로 바꾸게 되면 (0,1,2,...,9)로 바뀐다.
    3. x = 5,6,7           # tuple x를 list로 바꿀 수 있다.
       a = list(x)         # [5,6,7]이 된다.
    ```
    

### 패킹과 언패킹

- 패킹 : 여러개의 데이터를 하나의 변수에 할당하는 것
- 언패킹 : 컬렉션의 각 데이터를 각각의 변수에 할당하는 것

- 패킹 : `numbers = 3, 4, 5` ⇒ tuple형태로 numbers라는 변수에 저장
- 언패킹 : `a, b, c = numbers` ⇒ 묶음을 풀어 변수 상자에 저장 `numbers = (3,4,5)` 이고 a,b,c는 각각 3,4,5에 해당
- List에서도 마찬가지
- 패킹 : `numbers = [3, 4, 5]`
- 언패킹 : `a, b, c = numbers` ⇒ numbers=[3,4,5] 이며 a=3, b=4, c=5

- 만약 두 개의 변수가 있다고 가정할 때, 각각 변수의 값을 바꿔주고 싶을 때에도 사용할 수 있다.
- `a, b = b, a` ⇒ a 에는 b에 저장된 데이터가 들어가고, b에는 a에 저장되어 있던 데이터가 들어간다.
- 자바에서 temp 변수를 통해 자리를 바꾸는 것과 같음

### 튜플 함수

`a = 10, 20, 30, 40, 30`

| 특정값의 인덱스 구하기 | a.index(20) | 1 |
| --- | --- | --- |
| 특정값의 개수 | a.count(30) | 2 |
| 최대값, 최소값 | max(a), min(a) | 40, 10 |
| 합계 | sum(a) | 130 |