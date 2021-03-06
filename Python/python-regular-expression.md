# 정규표현식

---

복잡한 문자열을 처리할 때 사용하는 기법으로 , python만의 고유 문법이 아닌 문자열을 처리하는 모든 곳에서 사용한다.

## Why?

- 정규표현식을 사용하면 코드를 간소화 할 수 있다. 문자열에서 특정 문자를 찾거나, 규칙을 지정하는 경우에 자주 쓰인다.

## 메타 문자 (meta characters)

---

- 메타 문자란 원래 그 문자가 가진 뜻이 아닌 특별한 용도로 사용하는 문자
- 정규표현식에서 사용하는 메타 문자
  - ` . ^ $ * + ? { } [ ] \ | ( )`

### 문자 클래스 [ ]

- [] 사이의 문자들과 매치
- 정규표현식이 [abc]라면 이 포현식은 "a, b, c 중 한개의 문자와 매치"를 뜻한다.
- []안의 두 문자 사이에 하이픈(-)을 사용하면 두 문자 사이의 범위(From-To)를 의미한다
  - [a-zA-Z] - 알파벳 모두
  - [0-9] - 숫자

![regularexpressionliteral](../Image/pythonregularexpression.png)

### Dot(.)

- `.`
  - 모든 **문자**와 매치되는 메타문자이다.
- `a.b` vs `a[.]b`
  - `a.b`: 가운데 문자는 Dot 문자로 사용된다.
  - `a[.]b`: 문자 클래스 내에 Dot 메타 문자가 사용된다면 문자`.` 그대로를 의미한다.

### ?

직전에 있는 임의의 문자를 0회 또는 1회 반복한 패턴에 매치

### +

직전에 있는 임의 패턴을 1회 또는 그 이상의 수로 가급적 많이 반복하는 패턴에 대해서 매치

### findall

정규식을 만족하는 모든 문자열을 리스트 형태로 추출

### sub()

정규식에 해당하는 문자열을 특정 문자열로 대체
