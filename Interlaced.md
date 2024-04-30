
#### Challenge Description
---

*My image manipulation software crashed when I was editing and ended up corrupting the two files. Can you recover them?*

> *author: `Ork`*

![](Images/chal%20(2).png)

#### Walkthrough
---

The challenge's name is `interlaced`. What is `interlacing`?

`Interlacing` is a technique to fill the alternating lines of data in an image, helping to visualize the image before it is completely rendered.

In a normal image we see the first row of pixels, then the second line and so on as the image loads from top to bottom. This means we can't see much about the image until it is fully loaded. If we load every 2nd or 4th line of the image first then fill the remaining gaps, we will get a rough version of the image. (Our brain is very good at filling the gaps).

`Interlace` is helpful when the file is too large or the user has slow internet connection.

#### Understanding the problem
---

The question says the author was editing and accidentally corrupted two files. Here I think the two image files refer to two QR images. By intuition, I thought that the two images were `interlaced.`

So I looked for `deinterlacing tool` on online.

![](Images/Pasted%20image%2020240430231521.png)


After examining some links, I found a website called `G'MIC Online`

![](Images/Pasted%20image%2020240430231619.png)
After uploading the `chal.png` into that website, I clicked on the button called `Select Filter`

![](Images/Pasted%20image%2020240430231801.png)

You will find a list of filters.

![](Images/Pasted%20image%2020240430231842.png)

After looking into different filters, I clicked on `Repair`.

![](Images/Screenshot%202024-04-30%20231922.png)

Ah! `Deinterlace` interesting. Let's click on this.

![](Images/Pasted%20image%2020240430232057.png)

There are two algorithms we can see, one is `standard`, another one is `motion-compensated`

![](Images/Pasted%20image%2020240430232902.png)


Let's select `Motion-Compenstated` and render and then download.

We get this image :

![](Images/Pasted%20image%2020240430233056.png)

After scanning this QR code, we get this `r0gr4mm1ng_ch4ll3ng3!}`

As there are two images interlaced, this string is for one QR image. Let's find the other one.

![](Images/Pasted%20image%2020240430233441.png)

There is another option called `Deinterlace2x`. Let's do the same thing as before, `render` and click on the `Download` button.

We get this image :

![](Images/Pasted%20image%2020240430233557.png)

if you scan the QR code you will find this `iutctf{r34lly_ju57_4_p`

Basically this is the first part of the flag.

So the **flag** is : `iutctf{r34lly_ju57_4_pr0gr4mm1ng_ch4ll3ng3!}`
