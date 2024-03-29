## 📚 읽은 내용

### 암시적 변환
- 암시적 강제변환의 목적은 중요한 내용으로부터 주의를 분산시켜 코드를 집동사니로 가득채워버리는 장황함, 보일러플레이트, 불필요한 상세 구현을 줄이는것이다.
- 분명히 어떤 상횡에서는 코드 가독성 향상이라는 잠재적인 장점 이면에 코드를 다치게 할 온갖 해로운 성분이 꿈 틀대고 있을 수 있다. 따라서 버그로 도배한 코드를 짜려는 의도가 아니라면. 해로운 성분이 뭔 지 인식하고 피하는 방법 또한 확실히 알이아 한다.
- ||(논리OR) 및 &&(논리AND) 연산자는 실제로 결괏값이 논리 값(불리언)이 아니라 두 피연산자의 값들 중 하나 를 선택한다.
- '심벌->문자열' 명시적 강제변환은 허용되나 암시적 강제변환은 금지되며 시도만 해도 에러가 난다.

### 느슨한/엄격한 동등 비교
- 강제변환이 필요하다면 느슨한 동등 연산자(==)를, 필요하지 않다면 엄격한 동등 연산자 (===)를 사용하자.

## 📚 느낀점
- `암시적 강제변환 코드가 명시적 강제변환 코드보다 더 우아한 것 같다` 라고 했는데, 나는 너무 장황해지지만 않는다면 명시적이 더 이해하기 좋을거같다는 생각이든다.


## 📚 공유하고 싶은 부분(사이트)
