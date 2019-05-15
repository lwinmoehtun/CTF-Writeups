https://www.hackthis.co.uk/levels/crypt/1
>Decrypt the following text

>    tpyrcoow :ssap siht retne level siht etelpmoc oT .rewop niarb fo tol a yolpme ot deen lliw uoy ,cigol dna noitpyrced tuoba lla era slevel esehT .sihtkcah no slevel tpyrc eht ot emoclew ,olleH 

It's obvious that is a reversed string. I solved in python.

![alt crypt1](Resources/crypt%20lvl1.png)

## (OR)
If you are good at in loop,
```
flag = '' 
for i in msg:
    flag = i + flag   
print(flag)
```
## (OR)
You can also use slice.
```
>>>msg[::-1]
```
It's syntax is <tt>[start,stop,step]</tt>. I gave nothing to start and stop. So, it takes 0 as default. Step -1 denotes starting from end and stop at the start. Then, it becomes reverse string.





