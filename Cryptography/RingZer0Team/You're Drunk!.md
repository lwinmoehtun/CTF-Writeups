https://ringzer0ctf.com/challenges/274

>Ayowe awxewr nwaalfw die tiy rgw fklf ua xgixiklrw! Tiy lew qwkxinw. 

It's [ic](https://www.dcode.fr/index-coincidence) shows 0.06936. So, it is nearly equal to English text's ic. Moreover, msg is in text like structure.

Then, it used monoalphabetic substitution.

According to frequency analysis result, the most used character in the cipher text is 'w'.

In English language, the most frequent letter is <tt>e</tt>.

So, let's assume 'w'= <tt>e</tt>

The most frequent trigram in English is <tt>the</tt>.

You may found <tt>the</tt> in encrypted text as "--w".

Then, find the trigram that end with 'w'.

We found "rgw" and "lew".

Ok! let's try with "rgw" first.

Assume "rgw" = <tt>the</tt>.

w = <tt>e</tt>

r = <tt>t</tt>

g = <tt>h</tt>

Moreover, we found "ua" which can be assume to <tt>is</tt>

u = <tt>i</tt>

a = <tt>s</tt>

By inserting these characters, we can guess some words.

><tt>s</tt>yo<tt>e</tt>e  <tt>s</tt><tt>e</tt>xe<tt>e</tt><tt>t</tt>  n<tt>e</tt><tt>s</tt><tt>s</tt>lf<tt>e</tt>  die  tiy  <tt>the</tt> fklf  <tt>is</tt>  x<tt>h</tt>ixikl<tt>te</tt>!  tiy  le<tt>e</tt>  q<tt>e</tt>kxin<tt>e</tt>.
 
nwaalfw = n<tt>e</tt><tt>s</tt><tt>s</tt>lf<tt>e</tt>(Oh! it can be 'message')

n = <tt>m</tt>

l = <tt>a</tt>

f = <tt>g</tt>

Insert these characters once more:

Ahh! lew = <tt>a</tt>e<tt>e</tt>
It may be <tt>are</tt> because it is a common trigram.

e = <tt>r</tt>

awxewr = <tt>se</tt>x<tt>ret</tt> . Ya! it is <tt>secret</tt>.

x = <tt>c</tt>

Insert and we found

'die' = <tt>--r</tt>. It may be <tt>for</tt>

d = <tt>f</tt>

i = <tt>o</tt>

Insert them:

xgixiklrw = <tt>c</tt><tt>h</tt><tt>o</tt><tt>c</tt><tt>o</tt>k<tt>a</tt><tt>t</tt><tt>e</tt>

It's <tt>chocolate</tt>

k = <tt>l</tt>

So, fklf= <tt>glag</tt>

qwkxinw='q<tt>e</tt><tt>l</tt><tt>c</tt><tt>o</tt><tt>m</tt><tt>e</tt>'. It's <tt>welcome</tt>.

q = <tt>w</tt>

In this stage, the decrypter text is

>S--er secret message for -o- the glag is chocolate! You are welcome."

Now,it's easy to fill blanks.

>Super secret message for you the glag is chocolate! You are welcome.

Alas! there are some mistakes in the message.But,the name of the challenge is "You're drunk" and so, it is just mispelling. <tt>glag</tt> may be <tt>flag</tt>

Your flag is <tt>chocolate</tt>.








 
