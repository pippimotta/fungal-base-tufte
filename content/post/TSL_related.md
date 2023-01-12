+++
math = false 
title = "TLS communication"
type = "post"
date = "2023-01-12"
categories = ["lernen"]
+++

## How is the connection between client & server being secured in TLS? ##
It involves the use of public key and private key encryption, as well as the certification authority.

### General idea: 
- Any message encrypted w/ Kinoko's public key can only be decrypted with Kinoko's private key
- Any one with access to Kinoko's public key can verify that a message could only have been created by someone to Kinoko's private key
- A message encrypted with Public key is used for secrecy (as it could be only decrypted by private key)
- A message encrypted with Private key is used for authentication (a bit tricky but let's say who holds Kinoko's private key can be verified as Kinoko (kinoko is key itself --> key-no-ko🤡) ) 

### General process:
![](/images/tls-connection.png) 
{{<sidenote>}}Source: [How does HTTPS work?](https://www.youtube.com/watch?v=T4Df5_cojAs&t=281s) {{</sidenote>}}
{{< section "end" >}}

Takeout:
**The asymmetric encryption is used to secure the new shared secret key which is used to secure the following communication between the client and server (which is symmetric encryption (only one key)**

《====To Be Continued====