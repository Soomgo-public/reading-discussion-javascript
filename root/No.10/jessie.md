## π μ½μ λ΄μ©

- μ½νμ€νΈ κ·μΉ
  - μ€κ΄νΈ `{}` [κ°μ²΄ λ¦¬ν°λ΄, λ μ΄λΈ, λΈλ‘, κ°μ²΄ λΆν΄]
  - λ μ΄λΈ λ£¨ν? λ μ΄λΈ λΈλ‘?
  - else ifμ μ νμ  λΈλ‘
- μ°μ°μ μ°μ μμ
  - && κ° || λ³΄λ€ μ°μ μμκ° λλ€
- λ¨λ½ νκ°
  - `a && a.cool` μ boolean μ λ±μ§μλνκ³  a κ°μ λ±λλ€
  - (λΆνμν μ‘°κ±΄μ΄λ μ²μλΆν° `a.cool` λ‘ μ²΄ν¬νμ)
- λλν μ°μ 
  - && λ || λ³΄λ€, ||λ ?λ³΄λ€ κ°κ° μ°μ μμκ° λλ€
- κ²°ν©μ±
  - μ’μΈ‘μμ μ°μΈ‘μΌλ‘ μ‘°κ±΄μ κ²°μ μ§λλ€? λΈμ°~λΈμ°~

## π λλμ 

> **{} + []; //0  -> 0μ΄ λμ¬ μ κ° μκ΅¬λ..!**

```
[] + {}; // "[object Object]"
{} + []; //0
  ``` 
  

----

> **else if μ μ μ€μ μ μΌλ‘ λ΄κ° μκ°νκ²κ³Ό λ€λ₯Έ ννλ‘ νμ±λμ΄ μ­ν μ νκ³ μμκ΅¬λ!**

- μ€μ μ μΌλ‘ μ΄λ»κ² λμνλμ§λ₯Ό κ°μμ μΌλ‘ νμΈν΄μ μ‘°κΈ λ λΆλͺν μκ²λ κΈ°λΆ?
- `else ifλ₯Ό μ νν λ¬Έλ²κ·μΉμΈ μ λκ²¨μ§μ§ λ§μ..?!`
- <table>
<tr>
<td colspan="2" style="text-align: center">μΌμͺ½ λ¬Έλ²μ μ¬μ€ μ€λ₯Έμͺ½ μ²λΌ νμ±μ΄ λλ€~</td>
</tr>
<tr>
<td>

```

if(a) {
     ...
} else if (b) {
    ...
} else { 
    ... 
}

```

</td>
<td>

```
if (a) {
    ...
} else { 
    if (b) {
        ...
    } else {
        ...
    }
}
```

</td>
</tr>
</table>

- ~~μ.. μ΄λ κ² μ¬μ©ν λ°μ λ°λ‘ μ‘°κ±΄λ³λ‘ ν¨μλ₯Ό νΈμΆνλ νΈμ΄ νΈν λ―νλ€.~~

---
> **μ°μ°μ μ°μ μμ κ·μΉ? μ€μ€λ‘ μ¬κ°λ―Έμ μ½νμ§ μλλ‘ κ΄νΈλ₯Ό μ κ°μΈμ!**


## π κ³΅μ νκ³  μΆμ λΆλΆ(μ¬μ΄νΈ)
