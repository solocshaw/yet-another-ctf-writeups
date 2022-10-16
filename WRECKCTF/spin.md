### Challenge Description

crypto/spin

the classics.

oujp{xkurpjcxah_ljnbja_lryqna}

Author: BrownieInMotion

Attachments: [encrypt](attachments/spin/encrypt.py)

### Solution 

Looking at `encrypt.py` we see a function called `spin()` that takes the ordinal of characters in `flag.txt`, shifting the value, and outputting the corresponding unicode character:

```py
def spin(c, key):
    return chr((ord(c) - ord('a') - key) % 26 + ord('a'))
```

<details>
  <summary>Click to see flag</summary> 
  
    flag{obligatory_caesar_cipher}

</details>