https://www.hackthis.co.uk/levels/crypt/5

>Decrypt the following text

>    qoymlNlpY :ccdf lpy yzJ .qoh ln lxigqoh qlxlm eeiw zot ydpy gmipylnoC ,zot gmiyqdncyzo ho ydpy ci lniqk tN .lsie sooe tlpy ydpw yom ,smipy amd tdc tlpy ydpw tj lefolf gmigazb ho ydpy ci lniqk tN .tyicoiqzk ho ydpy ci lniqk tN .edminiqk d nd i clT 

The usual flag format is <tt>pass:***</tt>

But I don't find any of it in the msg . I only found :ccdf which is close to format. It's weird.
Lol, it's reversed.

Reverse it first.
```
>>> ''.join(reversed(msg))                                                                       
'Tlc i dn d kqinimde. Nt kqinl ic ypdy oh kzqiociyt. Nt kqinl ic ypdy oh bzagimg flofel jt wpdy yplt cdt dma ypims, moy wpdy yplt eoos eisl. Nt kqinl ic ypdy oh ozycndqyimg toz, Conlypimg ypdy toz wiee mlxlq hoqgixl nl hoq. Jzy ypl fdcc: YplNlmyoq'
```

It's ic is 0.05934. Nearly equal to that of english plain text(0.0667)
It's monoalphabetic substitution again.
This time, I'll use powerfull online [tool](https://www.quipqiup.com/).

```
Clues:
fdcc = pass

mode : statistics
```

>Yes i am a criminal. My crime is that of curiosity. My crime is that of judging people by what they say and think, not what they look like. My crime is that of outsmarting you, Something that you will never forgive me for. But the pass: TheMentor
