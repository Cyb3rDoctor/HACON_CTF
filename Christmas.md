# OSINT - Christmas



## Challenge description:
![challenge](https://user-images.githubusercontent.com/70543460/94372079-9f0ea980-0103-11eb-9c1a-455e40c1cb0c.png)

## Hints:
![hint](https://user-images.githubusercontent.com/70543460/94372091-ab930200-0103-11eb-8dd5-cbb3d637eaa0.png)

## Challenge files:
![Message](https://user-images.githubusercontent.com/70543460/94372103-bd74a500-0103-11eb-9906-0c6fe94a85b4.png)

## Solution:

The right corner in the bottom of the challenge image is interesting:
<br/><br/>
![dot code](https://user-images.githubusercontent.com/70543460/94372254-be5a0680-0104-11eb-9681-7f490873b38e.png)
<br/><br/>

That's called DotCode
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94372312-1bee5300-0105-11eb-80f5-699c52116715.png)
<br/><br/>

Search for DotCode scanners, and you will find some online tools, for example: (https://manateeworks.com/free-barcode-scanner)
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94372375-8dc69c80-0105-11eb-839b-45d2e7303f0a.png)
<br/><br/>

The decoded string is: **78 57 54 67 101 100 53 90**

<br/><br/>

Those are ASCII codes.

<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94372622-ec8d1580-0107-11eb-9900-727e7498ff00.png)
<br/><br/>

To convert them to characters, you can create a simple program to do that, or you can use online tools.

```C++
#include <iostream>
using namespace std;
int main()
{

int arr[8] = {78 , 57 , 54 , 67 , 101 , 100 , 53 , 90};

for (int i=0 ; i<8 ; i++)
  cout<<static_cast<char>(arr[i]);

return 0;
}
```

<br/><br/>
After converting the ASCII codes to characters, you will get: **N96Ced5Z**
<br/><br/>

According to the hint, you need to "paste" this string: **N96Ced5Z**...

And if you try pastebin, you will get the flag. (https://pastebin.com/N96Ced5Z)

<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94372737-ed727700-0108-11eb-9333-1c29a8c2da44.png)
<br/><br/>

**HACSEC{Y0u_aR3_1nt3ll1g3nT!!!}**
