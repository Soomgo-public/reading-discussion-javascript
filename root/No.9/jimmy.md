## ๐ ์ฝ์ ๋ด์ฉ
- ์ถ์ ๊ด๊ณ ๋น๊ต
    - ์ผ๋จ ๋ ํผ์ฐ์ฐ์์ ToPrimitive ์ฐ์ฐ
    - ๋ ๋ค ๋ฌธ์์ด์ด๋ฉด ์ฌ์ ์ ๋น๊ต๋ฅผ
    - ์ด๋ ํ์ชฝ์ด๋ผ๋ ๋ฌธ์์ด์ด ์๋ ๊ฒฝ์ฐ ๋ ๋ค ToNumber ์ฐ์ฐ
        - ์ซ์๊ฐ์ผ๋ก ๋ณํ ํ ๋น๊ต
    - a โค b ๋ a > b ๊ฒฐ๊ณผ๊ฐ์ ๋ถ์ ํ ๊ฐ
- ๋ฌธ๋ฒ
    - ๋ฌธ (Statement)
        - ํ๋ ์ด์์ ํํ์์ผ๋ก ์ด๋ฃจ์ด์ง๋ค
        - ํํ์ ๋ฌธ (Expression Statement)
            - ํ๋์ ํํ์์ด ๊ทธ ์์ฒด๋ก ์์ ํ ๋ฌธ์ ์ด๋ฃจ๋ ๊ฒฝ์ฐ
                - ex
                    - `b`
        - ๋ฌธ์ ํ๊ฐ ๊ฒฐ๊ณผ๋ ํญ์ ์๋ฃ ๊ฐ์ด๋ค
            - = ๋ชจ๋  ๋ฌธ์ ์๋ฃ ๊ฐ์ ๊ฐ์ง๋ค
        - ๋ฌธ์ ์๋ฃ ๊ฐ์ ํฌ์ฐฉํ๋ ๊ฑด eval() ํจ์๋ก ๊ฐ๋ฅํ๋ค
    - ํํ์ (Expression)
        - ๋ชจ๋  ํํ์์ ๋จ์ผํ, ํน์ ํ ๊ฒฐ๊ด๊ฐ์ผ๋ก ๊ณ์ฐ๋๋ค
        - ex
            - `3 * 6`
        - ํํ์์ ๋ถ์ ํจ๊ณผ๊ฐ ์๋ ๊ฒ๊ณผ ์๋ ๊ฒ์ผ๋ก ๋๋๋ค
            - ์๋
                - `a++`
                - `a = 3`
                - `delete`
            - ์๋
                - `a + 3`
## ๐ ๋๋์ 
- do ํํ์์ stage 1์ ๋จธ๋ฌผ๋ฌ ์๋ค๋ ๊ฒ์ ํ์ธ
- ๋ฌธ ์๋ฃ๊ฐ์ด ์ ์ค์ํ์ง๋ ์ ์ด์คฌ๋ค๋ฉด ์ข์์ ํ๋ฐ
    - ๋ด ์๊ฐ์๋ ๋ณ๋ก ์ค์ํ์ง ์์๋ณด์ธ๋ค
- delete ์ฐ์ฐ์
    - ํ๋กํผํฐ๋ฅผ ์ ๊ฑฐํ๋ ๊ฒ์ด ๋ถ์ํจ๊ณผ๋ผ๋
- ์ฐ์ฐ์๊ฐ โ๋ถ์ ํจ๊ณผ๋ฅผ ๊ฐ์ง๋คโ๋ผ๊ณ  ์๊ฐํด๋ณธ์ ์ด ์์๋ค. ํ ๋น ์ฐ์ฐ์๋ฉด ํ ๋น์ด ์ฃผ ํจ๊ณผ ์๋๊ฐ! ใใ

## ๐ ๊ณต์ ํ๊ณ  ์ถ์ ๋ถ๋ถ(์ฌ์ดํธ)
- Anย expressionย is any valid unit of code that resolves to a value.
![img.png](jimmy/img.png)

## ๊ฐ์ ์ฝ๋์ฌ๋ Expression์ด๋ Statement์ด๋๋ ๋งฅ๋ฝ์ ๋ฐ๋ผ ๊ฒฐ์ ๋  ์ ์๋ค.

[https://stackoverflow.com/a/36456009](https://stackoverflow.com/a/36456009)

It is possible for the same (textual) block of code to be considered both an expressionย *and*ย a statement depending on the context. E.g. the text snippetย `function f(){}`ย is an expression on line 1 and a statement in line 2 in the below code:

```
let g = function f() {};
function f() {};

```

So whether something is an expression or a statement cannot (in the general case) be determined by looking at a textual piece of code out of context; rather it is a property of a node in a syntax tree and can be decided only after the code is (mentally or actually) parsed.

## Expression์ผ๋ก์์ ํจ์๋ hoisting ๋์ง ์๊ณ  Statement๋ก์์ ํจ์๋ hoisting ๋๋ค
