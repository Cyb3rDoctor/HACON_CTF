# OSINT - Wigly Wigly Wack



## Challenge description:

![challenge](https://user-images.githubusercontent.com/70543460/94368972-c65b7b80-00ef-11eb-8b04-0bae8963eac1.png)

## Hints:

![hint1](https://user-images.githubusercontent.com/70543460/94369077-45e94a80-00f0-11eb-9acc-e916a9ec4247.png) ![hint2](https://user-images.githubusercontent.com/70543460/94369081-4f72b280-00f0-11eb-8604-816b33998e2d.png)

## Solution:



The challenge name reminds me with a website called **WiGLE** (https://wigle.net/)

<br/><br/>

![image](https://user-images.githubusercontent.com/70543460/94369208-0707c480-00f1-11eb-9b71-36b973e8a1a7.png)

<br/><br/>

So, what we have in the description (**00:04:0E:F2:3B:B5**) is the MAC address of a wireless hotspot.

And here are the steps to find that hotspot:



1. Go to https://wigle.net/search

2. Put (**00:04:0E:F2:3B:B5**) in the **BSSID/MAC** form, then click on **Query**

   

   ![image](https://user-images.githubusercontent.com/70543460/94369868-f2c5c680-00f4-11eb-8725-b2ed05b5cdc9.png)


<br/><br/>

You will see one search result:

![image](https://user-images.githubusercontent.com/70543460/94369907-24d72880-00f5-11eb-9b6b-2320fb94aa47.png)

<br/><br/>

And the flag is the SSID of that wireless hotspot.

**HACSEC{WLAN-f1364-Fritz}**
