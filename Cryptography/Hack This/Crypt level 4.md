https://www.hackthis.co.uk/levels/crypt/4
>Decrypt the following text

>    Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl 

It's [ic](https://www.dcode.fr/index-coincidence) is 0.0817 which is similar to that of English plain text. It is monalphabetic substituted English text.
Frequency analysis can break it.

I transfer cipher text to upper case. Decryped msg will be in lower case to be obvious.

<tt>$echo '...' | tr '[:lower:]' '[:upper:]'</tt>

Firstly, <tt>JHLL</tt> must be <tt>pass</tt> according to HackThis's format.

J = p

H = a

L = s

Due to [FA](https://www.dcode.fr/frequency-analysis), most frequent bigram in cipher txt is <tt>CL</tt>.

<tt>CL</tt> = <tt>is</tt> (<tt>CL</tt> can be <tt>is</tt> cause <tt>is</tt> is one of the most frequent bigram in English txt. Moreover, <tt>L</tt> is <tt>s</tt> as we found as above) 

C = i

Let's substitute them by translating respectively.

<tt>$echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLC' 'pasi'</tt>

we got:

>Di, GDis is a siRiSaN iKQa GZ SQWQS GUZ. GDis GiRQ QaYD SQGGQN is assiOMQK a spQYiAiQK NQSaGiZMsDip UiGD aMZGDQN SQGGQN. pass: iDaWQANiQMKs                           

<tt>Di</tt> may be <tt>hi</tt>

D = h

<tt>GDis</tt> = <tt>this</tt>

G = t

After substituting them, we get

>hi, this is a siRiSaN iKQa tZ SQWQS tUZ. this tiRQ QaYh SQttQN is assiOMQK a spQYiAiQK NQSatiZMship Uith aMZthQN SQttQN. pass: ihaWQANiQMKs

<tt>tZ</tt> = <tt>to</tt>

Z = o

<tt>tiRQ</tt> = <tt>time</tt>

R = m

Q = e

<tt>NQSatiZMship</tt> = <tt>relationship</tt>(frequent in daily life :P)

N = r

S = l

M = n

<tt>Uith</tt> = <tt>with</tt>

U = w

Let's substitute:
<tt>$ echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLCDGZRQNSMU' 'pasihtomerlnw'</tt>

>hi, this is a similar iKea to leWel two. this time eaYh letter is assiOneK a speYiAieK relationship with another letter. pass: ihaWeArienKs    

<tt>iKea</tt> = <tt>idea</tt>

K = d

<tt>leWel</tt> = <tt>level</tt> 

W = v

<tt>eaYh</tt> = <tt>each</tt>

<tt>assiOneK</tt> = <tt>assigned</tt>

O = g

if K = d

<tt>speYiAieK</tt> = <tt>specified</tt>

Y = c

A = f

Substitute them to get flag.
<tt>$ echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLCDGZRQNSMUKWOYA' 'pasihtomerlnwdvgcf'</tt>

>hi, this is a similar idea to level two. this time each letter is assigned a specified relationship with another letter. pass: ihavefriends                           




