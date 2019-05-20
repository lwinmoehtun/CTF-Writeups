https://ringzer0ctf.com/challenges/154

>Get the flag simple as that. Or ask @el_d33 the crypto master
>[Start the challenge](Resources/cryptoObject.png)

In the picture, I found a ribbbon(rope) with the letters.
It makes me remember a cipher which was used by chinese for thousands of year ago.
The rope with weird letters is wraped around a stick and it become readable words.
Of course! it is a [<tt>scytale</tt>](https://en.wikipedia.org/wiki/Scytale) cipher.

> Msg: GMODCDOOKCDBIOYDRMKDPQLDPVWYOIVRVSEOV 

It means absolute nothing!
The word <tt>FLAG</tt> should(or may) be include in the message.

I tried [rot](https://www.dcode.fr/rot-cipher) ciphers.
At rot 10, we got <tt>WCETSTEEASTRYEOTHCATFGBTFLMOEYLHLIUEL</tt> which includes characters <tt>F</tt>, <tt>L</tt>, <tt>A</tt>, <tt>G</tt>. Well, it seems right.

Let's try scytale cipher. I used [this](https://www.cryptool.org/en/cto-ciphers/scytale) to brute force the band.
At band 3, we got 
>WELCOMETOTHESCYTALETHEFLAGISBUTTERFLY

Flag is <tt>BUTTERFLY</tt>.

Band 3 is the most frequent one. You can try manually
```
WEL
COM
ETO
THE
SCY
TAL
ETH
EFL
AGI
SBU
TTE
RFL
Y
```

concat them: <tt>WELCOMETOTHESCYTALETHEFLAGISBUTTERFLY</tt>

Flag : <tt>BUTTERFLY</tt>

Gotcha!



