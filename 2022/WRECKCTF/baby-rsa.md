### Challenge 

there's p, but what's q?

Attachments: 

[challenge.py](attachments/baby-rsa/challenge.py)

[output.txt](attachments/baby-rsa/output.txt)

Author: BrownieInMotion

### Solution 

Looking at our `output.txt` file we have the values for $n$, $p$, and $c$. 

From `challenge.py` we see that our public key is `65537` and it uses the `pycryptodome` library. The function `getPrime()` returns a random N-bit prime number but we can use $p$ and $n$ to derive one of the prime factors, $q$. 

Once we have $q$ we can then derive the private key, $d$. 

More about the `pycryptodome` library and the use of `getPrime()` here: https://pycryptodome.readthedocs.io/en/latest/src/util/util.html

<details>
  <summary>Click to see flag</summary> 
  
    flag{omg_its_rsa}

</details>