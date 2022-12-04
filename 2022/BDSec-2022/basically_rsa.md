### Challenge Description

RSA cryptosystem uses modular arithmetic to create an asymmetric encryption system. However, there are some pitfalls and weakness. Can you exploit it?

N: `1280678415822214057864524798453297819181910621573945477544758171055968245116423923`

E: `65537`

C: `241757357533719849989659127349827982677055294256023833052829147857534659015212862`

Flag Format : BDSEC{fl4g_h3r3}

### Solution

$c=M^emodN$

We know $N$, $c$, and $e$ but not the private RSA key, $d$. How are we able to decrypt $M$?

It is possible to compute the value of $d$. 

More on RSA attacks here:

https://www.dcode.fr/rsa-cipher#q6

https://crypto.stanford.edu/~dabo/pubs/abstracts/RSAattack-survey.html

<details>
  <summary>Click to see flag</summary> 
  
    BDSEC{r54_i5_fUn_r16h7?}

</details>