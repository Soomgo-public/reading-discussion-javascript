## π μ½μ λ΄μ©

### κ°μ λ³ν
- κ°μ λ³νμ λμμ μ μκ³  μμΌλ, κ°μ λ³νμ μ’μ μ μ μκ³ μΆλ€.
- toString
  - λλ¬΄ ν¬κ±°λ μμ κ°μ μ§μ ννλ‘ λ°λ
  - JSON.stringify : JSON μμ κ°μ λͺ¨λ λ¬Έμμ΄ν κ° (JSON μμ  κ°μ΄ μλ κ²λ€μ undefined, ν¨μ(function), μ¬λ²(ES6λΆν°, symbol), νν μ°Έμ‘°(circular references))
- toBoolean
  - μ ν΄μ§ falsy κ° μ΄μΈμλ λͺ¨λ truthy 
  - κ°μ  λ³νμ μ μ©ν μ?
  ```typescript
  type Person = {
    name: string | null
  } 
  
  const getName = (person : Person) => {
    // if (person.name === null)
    if (!person.name) {
        console.log("μ΄λ¦μ΄ μλ€");
        return;
    }
    console.log(person.name);
  }
  
  const person = {
    name : null,
  };
  
  getName(person);
  ```
  - document.all -> documentGetElementById

### π λλμ 
- νμμ€ν¬λ¦½νΈ κ³΅λΆλ₯Ό μ΄μ¬ν νμ
- μλ. IE

### π κ³΅μ νκ³  μΆμ λΆλΆ(μ¬μ΄νΈ)



