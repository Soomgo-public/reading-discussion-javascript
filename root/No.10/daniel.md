## 📚 읽은 내용

### 콘텍스트 규칙
- 레이블 점프라는 특별한 형태의 goto 장치가 마련되어 있다.
- 만약 사용한다면, 뜻한 바를 상세한 주석으로 문서화 하길 바란다.

### 블록
- else if 같은건 없고, 문법의 숨겨진 특성이다. (신기..)

### 연산자 우선순위

```javascript
var a = 42, b;
b = ( a++, a);

a; // 43
b; // 43

b = a++, a;

a; // 43
b; // 42
```
- `=연산자`가 더 우선순위에 있어, 먼저 할당이 되는 상황
- && 연산자가 || 우선하여 처리 하기 때문에, 연산자 우선순위를 참고하여 작성하자!
- 물론 연산이 복잡한 것들은 따로 분리해서 작업하는게 좋은 것 같다.

### 단락 평가
- 만약 좌측 피연산자의  평가 결과만으로 전체 결과가 이미 결정될 경우 우측 피연산자의 평가를 건너뛴다.
- ||는 ? : 보다  각각 우선순위가 높다.
- 중용이 중요하다! 연산자 우선순위/결합성과 손으로 ( ) 를 감싸 주는 두 방법으로 적절히 배합하여 연산을 하자.

## 📚 느낀점
- 연산이 복잡한 프로그램을 다루지 않아서, 경험은 없지만 충분히 발생할 수 있다고 생각했다.
- 결국에는 개발자의 표현 방법에 따라 다르겠지만, 주석과 표현이 충분하다면 문제가 없지 않을까 감히 예상해봅니다.
 

## 📚 공유하고 싶은 부분(사이트)
- https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Operator_Precedence
