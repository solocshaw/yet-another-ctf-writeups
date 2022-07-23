### Challenge Description:

I just met a girl named Rejvi Khan. She told me to find her in social media. I searched on Facebook but didn't find her. I think she is using any other social media. Can you find her ?

Flag format : BDSEC{s0mething_here}

### Solution:

For this challenge we're going to user social media enumeration through spiderfoot. 

https://www.spiderfoot.net/documentation/

```py

cd spiderfoot-4.0 
python3 ./sf.py -m sfp_accounts -s "rejvikhan" -q 

```
We get the following:

```py 

Source             Type                      Data
SpiderFoot UI      Username                  rejvikhan
sfp_accounts       Account on External Site  Instagram (Category: social)
https://instagram.com/rejvikhan
sfp_accounts       Account on External Site  mastodon (Category: social)
https://mastodon.social/@rejvikhan
sfp_accounts       Account on External Site  Pinterest (Category: social)
https://www.pinterest.com/rejvikhan/
sfp_accounts       Account on External Site  Snapchat Stories (Category: social)
https://story.snapchat.com/s/rejvikhan
sfp_accounts       Account on External Site  Telegram (Category: social)

```

One of the above accounts has our flag.

<details>
  <summary>Click to see flag</summary>

BDSEC{yoU_goT_m3__oS1nT_I5_fUn_r1Gh7}

</details>