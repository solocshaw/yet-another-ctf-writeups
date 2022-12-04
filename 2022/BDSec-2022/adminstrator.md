### Challenge Description

What is the admin panel username & password?

Flag Format : BDSEC{username_password}

### Solution

Filtering our [capture.pcapng](attachments/capture.pcapng) file for http traffic we see a number of attempted logins:

We're looking for a login attempt that resulted in the `302 Found` status code:

![](img/wireshark-admin-panel-1.png)

Examinining the packet we find the following credentials: 

![](img/wireshark-admin-panel-2.png)

<details>
  <summary>Click to see flag</summary> 
  
    BDSEC{demo_demo}

</details>