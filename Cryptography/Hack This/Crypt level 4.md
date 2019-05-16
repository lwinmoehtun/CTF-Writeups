https://www.hackthis.co.uk/levels/crypt/4
>Decrypt the following text

>    Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl 

It's ic is 0.0817 which is similar to that of English plain text. It is monalphabetic substituted English text.
Frequency analysis can break it.

I transfer cipher text to upper case. Decryped msg will be in lower case to be obvious.
$echo '...' | tr '[:lower:]' '[:upper:]'

Firstly, JHLL must be pass according to HackThis's format.
J = p
H = a
L = s

Due to FA(frequency analysis), most frequent bigram in cipher txt is CL.
CL = is (CL can be is cause is is one of the most frequent bigram in English txt. Moreover, 'L' is 's' as we found as above) 
C = i

Let's substitute them by translating respectively.
$echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLC' 'pasi'

we got:
Di, GDis is a siRiSaN iKQa GZ SQWQS GUZ. GDis GiRQ QaYD SQGGQN is assiOMQK a spQYiAiQK NQSaGiZMsDip UiGD aMZGDQN SQGGQN. pass: iDaWQANiQMKs                           

Di may be hi
D = h

GDis = this
G = t

After substituting them, we get

hi, this is a siRiSaN iKQa tZ SQWQS tUZ. this tiRQ QaYh SQttQN is assiOMQK a spQYiAiQK NQSatiZMship Uith aMZthQN SQttQN. pass: ihaWQANiQMKs

tZ = to
Z = o

tiRQ = time
R = m
Q = e

NQSatiZMship = relationship(frequent in daily life :P)
N = r
S = l
M = n

Uith = with
U = w

Let's substitute:
$ echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLCDGZRQNSMU' 'pasihtomerlnw'

hi, this is a similar iKea to leWel two. this time eaYh letter is assiOneK a speYiAieK relationship with another letter. pass: ihaWeArienKs    

iKea = idea
K = d

leWel = level 
W = v

eaYh = each

assiOneK = assigned
O = g

if K = d
speYiAieK = specified
Y = c
A = f

Substitute them to get flag.
$ echo 'Dc, gdcl cl h lcrcshn ckqh gz sqwqs guz. Gdcl gcrq qhyd sqggqn cl hllcomqk h ljqycacqk nqshgczmldcj ucgd hmzgdqn sqggqn. Jhll: cdhwqancqmkl' | tr '[:lower:]' '[:upper:]' | tr 'JHLCDGZRQNSMUKWOYA' 'pasihtomerlnwdvgcf'

hi, this is a similar idea to level two. this time each letter is assigned a specified relationship with another letter. pass: ihavefriends                           




