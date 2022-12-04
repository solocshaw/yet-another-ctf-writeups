### Challenge Description

I convert plain text to cipher text by using Cryptocode library . Always Remember BDSEC is a KEY .

Attachments

[cipher.txt](attachments/cipher.txt)

Flag Format : BDSEC{fl4g_h3r3}

### Solution

To decrypt our cyphertext we're going to install the cryptocode python library: https://pypi.org/project/cryptocode/

Once we've installed cryptocode we'll import it into our interactive shell and use the following function:

```python

myDecryptedMessage = cryptocode.decrypt("cyphertext", "key")

```

```python
>>> import cryptocode
>>> myDecryptedMessage = cryptocode.decrypt("c00EtfL9GPq2EItQrkFyPKIMfVFZy0O4ssXtr/V2Io7NMbNS*Brue6Cex4JuWkWU0lUEK2w==*f8EsezuHu2WBstRDlWZiLg==*CZ/4FNMavWZu3kznPrAyeg==", "BDSEC")
>>> print(myDecryptedMessage) #print(flag)
```

<details>
  <summary>Click to see flag</summary> 
  
    BDSEC{cryp70_and_pyth0n_ar3_aw3s0me}

</details>

