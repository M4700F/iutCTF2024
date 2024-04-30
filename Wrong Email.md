
#### Challenge Description

*I have just received a really offensive email from this address `avalon8973@gmail.com`. After a bit of digging around, I found that the owner of this mail is moving a lot. Can you tell me where he was last?*

*N.B. The flag will be the name of the last visited district.*

*Flag format: `iutctf{District}`*

*author: `Mohammed Sami Khan`*

---
#### Walkthrough


First what came in my mind that is there any online tool that can trace email address?. If you search like `email location finder` or something like this, you will find many website that can find the location of the email. But most of them are paid.

Even I found a chrome extension called `mailtag` that can give the location of the email address if an email with `mailtag` on was opened by the user. I did send a mail to `avalon8973@gmail.com` 
hoping that `avalon` would open it :)

Another thought came to my mind that why not search the `avalon8973` on google advanced search or something because this `avalon8973` seems like a username.

I searched `advanced search` and found `Search Advanced - Twitter`. In many CTFs, I found that , in the `osint` category, if you are searching some info about someone in a challenge, you will find it in the twitter.

Now let's search the  `avalon8973` part in `twitter advanced search`.

![](Images/Pasted%20image%2020240430204655.png)

You will find this account only.

![](Images/Pasted%20image%2020240430204758.png)

Now if you go into the account, you will see photo of a bus of `SUST`. So `avalon` was last in `Sylhet`.

**Flag : `iutctf{Sylhet}`**

![](Images/Pasted%20image%2020240430205001.png)