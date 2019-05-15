https://www.hackthis.co.uk/levels/crypt/2
>Decrypt the following text

>    Aipgsqi fego, xlmw pizip mw rsx ew iewc ew xli pewx fyx wxmpp rsx xss gleppirkmrk. Ws ks elieh erh irxiv xlmw teww: wlmjxxlexpixxiv 

   It's text like structure and calculated [ic](https://www.dcode.fr/index-coincidence) is 0.07491(nearly equal to that of plain text).
So, it can be substitution cipher or shift cipher(caesar cipher).
As it's low point challenge, let's try shifts.

<tt>teww: wlmjxxlexpixxiv</tt> may be <tt>pass: ***************</tt>. So, it shifts from <tt>t</tt> to <tt>p</tt>. That is shift 22 on caesar cipher.

<tt>$ echo Aipgsqi fego, xlmw pizip mw rsx ew iewc ew xli pewx fyx wxmpp rsx xss gleppirkmrk. Ws ks elieh erh irxiv xlmw teww: wlmjxxlexpixxiv | caesar 22</tt>

Welcome back, this level is not as easy as the last but still not too challenging. So go ahead and enter this pass: shiftthatletter
