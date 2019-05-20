I extract tar file and searched password in folders as follows: 
$ grep -i -r pass 

And I found cpassword.
cpassword="PCXrmCkYWyRRx3bf+zqEydW9/trbFToMDx6fAvmeCDw"

Google: cPassword is the name of the attribute that stores passwords in a Group Policy Preference item.

So, use gpp decrypt.
If you are using kali, there is gpp-decrypt tool.
But, I used a ruby file to decrypt it.
