https://ringzer0ctf.com/challenges/114

```
VoiCI unE SUpeRbe reCeTtE cONcontee pAR un GrouPe d'ArtistEs culinaiRe, dONT le BOn Gout et lE SeNs de LA cLasSe n'est limIteE qUe par LE nombre DE cAlOries qU'ils PeUVEnt Ingurgiter. Ces virtuoses de la friteuse vous presente ce petit clip plein de gout savoureux !!

We hijack the Bacon Bacon Truck in San Francisco!


The cure for your worst
Hangovers and more: Bacon
True: Science says so
```
I saved the msg in [bacon.txt](Resources/bacon.txt)

The message was composed with Capital & Small letters. It can be assume as two types of letter. The cipher that uses two types of letter is [baconian cipher](http://practicalcryptography.com/ciphers/baconian-cipher/).

Ahh! of course, <tt>bacon</tt> is described as hint.

Usual one may be <tt>AABBBABBABABAB...</tt>

So, let's change to it:

Let's assume Capital letter as <tt>A</tt> and Small letter as </tt>B</tt>. Ignore(remove) <tt>spaces</tt>, <tt>.</tt>, <tt>,</tt>, <tt>'</tt>, <tt>!</tt>

Here we go!

![bacon](Resources/Bacon.png)

more about [tr](https://www.geeksforgeeks.org/tr-command-in-unix-linux-with-examples/) command

more about [sed](https://www.geeksforgeeks.org/sed-command-in-linux-unix-with-examples/) command

You can use <tt>sed "s/[A...Z]/A/g"</tt> instead of <tt>tr</tt>.

Now, we can solve with baconian cipher. The logic is
```
A = AAAAA   #It is similar to 00000(AAAAA),00001(AAAAB),00010(AAABA),...
B = AAAAB
C = AAABA
D = AAABB
E = AABAA
F = AABAB
G = AABBA
H = AABBB
I/J=ABAAA
K = ABAAB
L = ABABA
M = ABABB
N = ABBAA
O = ABBAB
P = ABBBA
Q = ABBBB
R = BAAAA
S = BAAAB
T = BAABA
U/V=BAABB
W = BABAA
X = BABAB
Y = BABBA
Z = BABBB
```

You can substitute each 5 letter to one decrypted cipher.
After knowing this, I used online [tool](https://www.dcode.fr/bacon-cipher) to decrypt it.

>THEFLAGISBACONANDJACKDANIELS

!!! Others are not part of the flag.
