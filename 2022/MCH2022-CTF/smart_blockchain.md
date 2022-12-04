### Challenge Description

On this smart blockchain, you can upload your code to be run by all the miners! Isn't that magic. But why do we bother with all that planet-melting hashing? Nobody knows.

Get the server to run your Python code and read the flag from /flag on smartblockchain.ctf.zone:8333.

Source:

```python
import hashlib
import sys
import os

def is_printable_ascii(c):
    string = chr(c)

    return string.isascii() and string.isprintable()


def make_payload(line, salt):
    hashed = hashlib.md5((salt + line).encode("utf8")).digest()

    code = filter(is_printable_ascii, hashed)

    return bytes(code).decode("ascii")


salt = os.urandom(8).hex()

print(f"Here is your salt: {salt}")

sys.stdout.flush()

payload = ""

for line in sys.stdin:

    if line[-1] == "\n": line = line[:-1]

    payload += make_payload(line, salt)

eval(payload)
```

### Solution

