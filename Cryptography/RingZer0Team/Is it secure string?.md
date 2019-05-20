https://ringzer0ctf.com/challenges/55

```
I found an encrypted password and the key. Recover the pass!

Password:
76492d1116743f0423413b16050a5345MgB8AEEAYQBNAHgAZQAxAFEAVAB
IAEEAcABtAE4ATgBVAFoAMwBOAFIAagBIAGcAPQA9AHwAZAAyADYAMgA2AD
gAMwBlADcANAA3ADIAOQA1ADIAMwA0ADMAMwBlADIAOABmADIAZABlAGMAM
QBiAGMANgBjADYANAA4ADQAZgAwADAANwA1AGUAMgBlADYAMwA4AGEAZgA1
AGQAYgA5ADIAMgBkAGIAYgA5AGEAMQAyADYAOAA=


Key:
(3,4,2,3,56,34,254,222,205,34,2,23,42,64,33,223,1,34,2,7,6,5,35,12)
```

At first, I thought it was base 64 but didn't work.
So, I google secure string.
I found some [solutions](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/convertto-securestring?view=powershell-6).

Open powershell:

![secure string](Resources/securestring.png)

Then, got the flag.

>FLAG-5tguasm48
