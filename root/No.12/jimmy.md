## ๐ ์ฝ์ ๋ด์ฉ
- ์ค์ฝํ
    - ํน์  ์ฅ์์ ๋ณ์๋ฅผ ์ ์ฅํ๊ณ  ๋์ค์ ๊ทธ ๋ณ์๋ฅผ ์ฐพ๋ ๋ฐ ์ฌ์ฉ๋๋ ๊ท์น
- ์๋ฐ์คํฌ๋ฆฝํธ๋ ์ฌ์ค โ์ปดํ์ผ๋ฌ ์ธ์ดโ. ๊ทธ๋ฌ๋ ์ ํต์ ์ธ ์ปดํ์ผ๋ฌ ์ธ์ด์๋ ๋ค๋ฅด๋ค
    - ์ ํต์ ์ธ ์ปดํ์ผ๋ฌ ์ธ์ด์์๋ ๋ณดํต ์์ค ์ฝ๋๊ฐ ์คํ๋๊ธฐ ์ ์ 3๋จ๊ณ๋ก ์ด๋ฃจ์ด์ง๋ Compilation ๊ณผ์ ์ ๊ฑฐ์น๋ค
        - Tokenizing & Lexing
            - ๋ฌธ์์ด์ ํ ํฐ์ผ๋ก ๋ง๋๋ ๊ณผ์ 
        - Parsing
            - ํ ํฐ ๋ฐฐ์ด์ ๋ฌธ๋ฒ ๊ตฌ์กฐ๋ฅผ ๋ฐ์ํ ์ค์ฒฉ ์์๋ฅผ ๊ฐ๋ ํธ๋ฆฌ ํํ๋ก ๋ฐ๊พธ๋ ๊ณผ์ 
            - ๋ง๋ค์ด์ง ํธ๋ฆฌ๋ฅผ ์ถ์ ๊ตฌ๋ฌธ ํธ๋ฆฌ(AST = Abstract Syntax Tree)๋ผ๊ณ  ๋ถ๋ฅธ๋ค
        - Code Generation
            - AST๋ฅผ ์คํ ์ฝ๋๋ก ๋ฐ๊พธ๋ ๊ณผ์ 
    - ์๋ฐ์คํฌ๋ฆฝํธ ์์ง์
        - Compilation์ ์ฝ๋๋ฅผ ์ต์ ํ ํ๋ค
            - ๋ถํ์ํ ๋ถ๋ถ์ ์ญ์ ํ๋ ๋ฑ
        - Compilation์ ์ฝ๋๊ฐ ์คํ๋๊ธฐ ์ง์ ์ ์ํํ๋ค
            - ์ ํต์ ์ธ ์ปดํ์ผ๋ฌ์์๋ Compilation์ ๋ฏธ๋ฆฌ ์ํ
            - ๋ฐ๋ผ์ Compilation์ ์๊ฐ์ ๋ง์ด ์ฌ์ฉํ  ์ ์๊ธฐ ๋๋ฌธ์ ๊ฐ์ฅ ๋น ๋ฅธ ์ฑ๋ฅ์ผ๋ก Compilation์ ์ํํ๊ธฐ ์ํด ์ฌ๋ฌ ํธ๋ฆญ์ ์ฌ์ฉํ๋ค
- ์ปดํ์ผ๋ฌ๊ฐ ํ๋ ์ผ: ์ค์ฝํ
    - ๋ณ์ ์ ์ธ์ ๋ง๋๋ฉด ์ค์ฝํ์ ์ ์ธํ๋ค. ์ด๋ฏธ ์๋ค๋ฉด ์ ์ธ์ ๋ฌด์ํ๋ค
    - ๊ทธ๋ฆฌ๊ณ  ๋์๋ฌธ์ ์์ง์ด ์คํํ  ์ ์๋ ์ฝ๋๋ก ๋ณํํ๋ค
- ๋ณ์๋ฅผ ์ฐพ๋ ๋ ๊ฐ์ง ๊ฒ์: LHS, RHS
    - LHS
        - ๋์ํ  ๋์์ด ๋๋ ๋ณ์๋ฅผ ์ฐพ์ ๋ ์ฌ์ฉ
        - ๋ณ์ ์ปจํ์ด๋ ์์ฒด๋ฅผ ์ฐพ์
        - ๋์
            1. ํ์ฌ ์ค์ฝํ์์ ์ฐพ๋๋ค
            2. ์์ผ๋ฉด ๋ฉ์ถ๊ณ  ์์ผ๋ฉด ๋ถ๋ชจ ์ค์ฝํ์์ ์ฐพ๋๋ค
            3. 2๋ฒ์ ๊ธ๋ก๋ฒ ์ค์ฝํ์์ ์ฐพ๊ฒ๋  ๋๊น์ง ๋ฐ๋ณตํ๋ค
            4. ๋๊น์ง ์ฐพ์ง ๋ชปํ ๊ฒฝ์ฐ, Strict Mode๋ผ๋ฉด ReferenceError๋ฅผ ๋์ง๊ณ , ์๋๋ผ๋ฉด ๊ธ๋ก๋ฒ ์ค์ฝํ์ ๋ณ์๋ฅผ ํ๋ ์ถ๊ฐํ๋ค
    - RHS
        - ๋์ํ  ๊ฐ์ด ๋๋ ๋ณ์๋ฅผ ์ฐพ์ ๋ ์ฌ์ฉ
        - ๋ณ์ ๊ฐ์ ์ฐพ์
        - ๋์
            1. ํ์ฌ ์ค์ฝํ์์ ์ฐพ๋๋ค
            2. ์์ผ๋ฉด ๋ฉ์ถ๊ณ  ์์ผ๋ฉด ๋ถ๋ชจ ์ค์ฝํ์์ ์ฐพ๋๋ค
            3. 2๋ฒ์ ๊ธ๋ก๋ฒ ์ค์ฝํ์์ ์ฐพ๊ฒ๋  ๋๊น์ง ๋ฐ๋ณตํ๋ค
            4. ๋๊น์ง ์ฐพ์ง ๋ชปํ ๊ฒฝ์ฐ ReferenceError๋ฅผ ๋์ง๋ค
            5. ์ฐพ์์ง๋ง ์ฐพ์ ๊ฐ์ผ๋ก ๋ถ๊ฐ๋ฅํ ์ผ์ ํ๋ ค๊ณ  ํ๋ ๊ฒฝ์ฐ TypeError๋ฅผ ๋์ง๋ค
    - ํจ์ ์ ์ธ๋ฌธ(function ์ ์ธ)์๋ LHS ๊ฒ์์ด ์ฌ์ฉ๋์ง ์๋๋ค
        - ์์ง์ด ํจ์๊ฐ์ ๋์ํ๋ ๊ณผ์ ์ด ๋ถํ์ํ๊ธฐ ๋๋ฌธ์
## ๐ ๋๋์ 
- arrow function์ธ ๊ฒฝ์ฐ LHS ๊ฒ์์ด ์ฌ์ฉ๋  ๊ฒ๋ง ๊ฐ์๋ฐ ๊ด๋ จ ๋ด์ฉ์ ์ ๋ชป์ฐพ๊ฒ ๋ค. ๋ค์ ๊ธฐํ์

## ๐ ๊ณต์ ํ๊ณ  ์ถ์ ๋ถ๋ถ(์ฌ์ดํธ)
