## π μ½μ λ΄μ©

### 4.5.2 μΆμ λλ± λΉκ΅

```javascript
var a = 42;
var b = "42";

a === b; // false
a == b; // true
```
- ν΄λΉ μλ¦¬λ ToNumber() κ°μ  λ³ν μΌμ΄λ ν λΉκ΅

```javascript
var a = "42";
var b = true;

a == b; // false
```
- μμ μλλ ToNumber() κ°μΌλ‘ κ°μ λ³νμ΄ λμ΄, "42"λ true > 1μ κ°μ΄λ―λ‘ λ€λ₯΄λ€.

> κ²°λ‘ μ μΌλ‘ μ μ¬λ‘λ₯Ό ν΅ν΄ μλμ κ°μ λ°©λ²μ μ°λκ² μ’λ€.
```javascript
// μμμ 
if (a)


// λͺμμ 
if (!!a)
//

// λͺμμ 
if (Boolean( a ))
//
```
### 4.5.3 ν¬κ· μ¬λ‘
- λ€μ΄ν°λΈ νλ‘ν νμμ λ³κ²½νλ€λ©΄... valueOf κ°μ κ° > μ νν λΉκ΅κ° λμ§ μλλ€. μλνλ©΄ κ°μ²΄ κ²½μ° μμκ°μΌλ‘ λ³νν  λ valueOfμ μ¬μ©νκΈ° λλ¬Έμ΄λ€.
- κ°μ λ³νμ΄ μ¬κ°ν λ¬Έμ κ° λ  κ²½μ°λ 7κ°μ§ μ΄λ€. νμ§λ§ λλ¨Έμ§λ μ΄λ‘ μ μΌλ‘ μ€λͺμ΄ κ°λ₯νλ€.

- νΌμ°μ°μ μ€ νλκ° true/false μΌ κ°λ₯μ±μ΄ μμΌλ©΄ μ λλ‘ == μ°μ°μλ₯Ό μ°μ§ λ§μ
- νΌμ°μ°μ μ€ νλκ° [], " ", 0μ΄ λ  κ°λ₯μ±μ΄ μμΌλ©΄ κ°κΈμ  == μ°μ°μλ μ°μ§ λ§μ

### π λλμ 
- λ€μ΄ν°λΈ νλ‘ν νμμ λ³κ²½ν κ²½νμ μμ§λ§, μ‘°μ¬ν΄μΌνκ³  μλ²½ν λμμ μ΄ν΄ νμ λ μ¬μ©νμ§ μμκΉλΌλ μκ°μ νλ€.
- κ°μ λ³ν κ²½μ°λ μλ²½νκ² μ΄ν΄ν ν μ¬μ λ₯Ό μ λκ²μ΄ νμμμλ λλ²κΉμμλ μ’μ κ² κ°λ€κ³  λ€μ νλ² μκ°νκ² λμλ€.
- λΉκ΅ μ°μ°μ ν  λ, λμνλ μμμ λν΄μ μκ°ν΄λ³Έ κ² κ°μ μλ‘μ λ€.

### π κ³΅μ νκ³  μΆμ λΆλΆ(μ¬μ΄νΈ)
- 