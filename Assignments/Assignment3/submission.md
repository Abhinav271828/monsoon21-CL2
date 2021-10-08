---
title: Computational Linguistics 2 (CL3.202)
subtitle: |
          | Monsoon 2021, IIIT Hyderabad
          | Assignment 3
author: Abhinav S Menon
header-includes:
- \newfontfamily\malayalamfont{MalayalamMN}
---

Note on notation: Capital `E` has been used to indicate "there exists", *e.g* `Ex (x PRED)` is to be read as "there exists x that satisfies `PRED`", or "there is an x such that x satisfies `PRED`".

# Question 1
* **When the lockdown was declared, John went to Bombay or Pune and Mary went to Delhi.**  
    [assuming the "when X, Y" construction is equivalent to "X and Y"]  
    `(l DECLARED) & ((j GOTO b) V (j GOTO p)) & (m GOTO d)`

* **I don't remember, but either John or Mary went to Bombay and Susan went to Delhi.**  
    [assuming "either X or Y" represents the inclusive OR, *i.e.*, at least one of X and Y is true]  
    `~(i REMEMBER) & ((j GOTO b) V (m GOTO b)) & (s GOTO d)`

* **John will not marry Mary if he doesn't get a job.**  
    [since "a job" is indefinite, it has been expressed as "if there does not exist a job $w$ such that John gets $w$"]  
    `~(Ew (j GET w)) -> ~(j MARRY m)`

* **John will marry Mary or Susan and settle abroad.**  
    ["settle abroad" is considered as an atomic predicate]  
    `((j MARRY m) V (j MARRY s)) & (j SETAB)`

* **John will not take the job and Mary will either study further or teach children.**  
    [like in (c), "children" is indefinite and therefore it has been expressed as "there will exist children $c$ such that Mary teaches $c$"]  
    `~(j TAKE w) & ((m STUFUR) & (Ec (m TEACH c)))`

The glossary is as follows:  
`l`: the lockdown  
`j`: John  
`b`: Bombay  
`p`: Pune  
`m`: Mary  
`d`: Delhi  
`i`: I (*i.e.* the speaker)  
`s`: Susan  

`SETAB`: settle abroad  
`STUFUR`: study further

# Question 2
Let the boy in the red shirt be Ravi, the boy in the yellow shirt Yash, the girl in the pink dress Preetha, and the girl in the blue dress Bindu.  

* **Ravi is jumping.**  
    `r JUMP`

* **The trees are green.**  
    `t GREEN`

* **Yash is pulling the cart and cart contains the flowers.**  
    `(y PULL c) & (c CONTAIN f)`

* **Bindu is reading the book.**  
    `(b READ k)

* **Bindu is sitting on the first swing and the second swing is empty.**  
    `(b SITON s1) & (s2 EMPTY)`

* **If the weather is rainy, Bindu will not read the book.**  
    `w RAINY -> ~(b READ k)`

* **Either Ravi and Preetha will play or Preetha will leave.**  
    `((r PLAY) & (p PLAY)) V (p LEAVE)`

* **If Preetha calls Bindu, she will not read the book.**  
    `p CALL b -> ~(b READ k)`

* **Preetha is running.**  
    `p RUN`  

* **Ravi is happy if and only if the sun is shining.**  
    `s SHINE <-> r HAPPY`


The glossary is as follows:  
`r`: Ravi  
`t`: the trees  
`y`: Yash  
`c`: the cart  
`f`: the flowers  
`b`: Bindu  
`k`: the book  
`s1, s2`: the first and second swings  
`w`: the weather  
`p`: Preetha  
`s`: the sun

# Question 3
## Set 1
* **Virat hit the ball.**

* **The ball was hit by Virat.**

* **Virat is the one who hit the ball.**

All these sentences have the common logical formula `v HIT b`.

## Set 2
* **The ball broke the window.**

* **The window broke because of the ball.**

* **The window was broken by the ball.**

All these sentences have the common logical formula `b BREAK w`.

# Question 4
* **John went to Trivandrum or Mary went to Hyderabad and Susan went to Chennai.**  
    Interpretation 1: `(j GOTO t) V ((m GOTO h) & (s GOTO c))`  
    Interpretation 2: `((j GOTO t) V (m GOTO h)) & (s GOTO c)`

* **John and Mary are married.**  
    Interpretation 1: `(Ex (j MARRY x)) & (Ey (m MARRY y))`  
    Interpretation 2: `j MARRY m`

* **Both John and Mary don't know.**  
    Interpretation 1: `~(j KNOW) & ~(m KNOW)`  
    Interpretation 2: `~((j KNOW) & (m KNOW))`
