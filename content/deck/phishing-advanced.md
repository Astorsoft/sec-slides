+++
title = "Advanced phishing techniques"
type="slide"
theme = "kindred"
lang="en"
+++
<!-- .slide: data-background="http://i.imgur.com/iXrdLRm.jpg" data-state="blur shadow" -->

# Advanced Phishing techniques

### And how to defend against them

*Morgan Hotonnier - Group Security*

> <*f*> for fullscreen, <*space*> for next slide
---
<!-- .slide: data-background="http://i.imgur.com/q6iIF7t.jpg" data-state="box shadow" -->

## Previous training was too easy!

---
<!-- .slide: data-background="http://i.imgur.com/iXrdLRm.jpg" data-state="dim" -->

## Advanced techniques

- Email Hijack
- Typosquatting
- IDN Homograph
- RTL technique
- Shortener and redirects
- File extension tricks
- Dangerous files
- httpS = Secure?
- The line of death
- Tabnapping

---
<!-- .slide: data-background="http://i.imgur.com/0V1Gtro.jpg" data-state="dim" -->

## Email Hijack

If your friend got hacked

![friend hacked](http://imgur.com/qp1GiCG.jpg)

attacker doesn't even need to spoof anything

---
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="shadow blur" -->

## Typosquatting

> Please visit <span class="fragment highlight-red">rn</span>icrosoft.com for more details

note:

Sometimes it is very difficult to differentiate visually some letters, or groups of letters, from others, typosquatteur will use it to make their phishing link looks legit
___
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="dim" -->

## Typosquatting

> Sorry, I meant  mi<span class="fragment highlight-red">rc</span>osoft.com

<iframe src="https://geon.github.io/programming/2016/03/03/dsxyliea" width="800" height="400"></iframe>

Note:

Another easy way is to invert two letters in the url, if you don't look carefully you may not even notice it
___
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="dim" -->
## Typosquatting

> Damn! I meant micr<span class="fragment highlight-red">p</span>soft.com

![big thumb](https://cdn.meme.am/instances/39718882.jpg)

Note:
Finally, if they just want you to go there by yourself, they can try to squat common typing mistake.

---
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## Homographs

Wikip<span class="fragment highlight-red" data-fragment-index="1">e</span>di<span class="fragment highlight-green" data-fragment-index="2">a</span> != Wikip<span class="fragment highlight-red" data-fragment-index="1">&#1077;</span>di<span class="fragment highlight-green" data-fragment-index="2">&#1072;</span>

Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## Homographs

Let's put them next to one another

- <font color="green">e</font><font color="red">&#1077;</font>
- <font color="green">a</font><font color="red">&#1072;</font>


Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## How can I seriously spot that?!

- Thanksfully browsers got your back
 - Link are displayed in **punycode**
 - This makes a text like this : http://www.pa&#1091;pal.com
 - Look like this: http://www.xn--pypal-4ve.com/

![Punycode example](http://i.imgur.com/dxSJqSX.png)


Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
---
<!-- .slide: data-background="http://i.imgur.com/21XrAzX.jpg" data-state="dim" -->

## URL Bar RTL attack

> erehwyreve thgir ot tfel morf daer t'nod ew esuaceB

note:
http://www.rafayhackingarticles.net/2016/08/google-chrome-firefox-address-bar.html?m=1
___
<!-- .slide: data-background="http://i.imgur.com/21XrAzX.jpg" data-state="dim" -->

### RTL Techniques

The link http://عربي.امارات/google.com/test/test/test was displayed like this

![RTL Attack](http://i.imgur.com/sR2cLnN.png)

It's patched...<span class="fragment highlight-red">for now</span>.

note:
http://www.rafayhackingarticles.net/2016/08/google-chrome-firefox-address-bar.html?m=1

---
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="shadow" -->

### Redirections

___
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="dim" -->

## Shortener

> Because http://tiny.cc/recover-gmail-password looks safe, right?

___
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="dim" -->

## Open redirects

What about this one? <a href="#">http://www.ebay.com/totally/legit/long/url/<span class="fragment highlight-green">redirect.php?url=http://malicious.example.com</span></a>

Note:
Can also be done with javascript on vulnerable websites (XSS)
___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## Defense?

You could just click and look at the final URL...

...but if this is a drive-by download malware

you may still get infected.

___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

You can also use "link expander" services such as http://www.linkexpander.com/

![link expander example](http://i.imgur.com/ByM4PuW.png)

---
<!-- .slide: data-background="http://i.imgur.com/TVqYFqF.jpg" data-state="dimblur shadow"-->

## File extensions

> Double click to open nude-pics.jpg<font color="gray"><span class="fragment highlight-red">.exe</span></font>

![double extension trick](http://i.imgur.com/WX7NY9M.png)


---
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="shadow"-->
## Dangerous files

___
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="dimblur shadow"-->

## Dangerous files

> If it does not end with .exe, I can open it safely, right?

___
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="dim"-->

## Dangerous files

- It's a bit more complicated
- There is more than 50 dangerous extensions
 - .pif, .msi, .com, .scr, .msc, .jar, .bat, .cmd, .vb, .js, .ps1, .msh, .lnk, .inf, .reg
 - But also .svg, .doc, .xls, .ppt...

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Defense?

- Prefer the white list approach over the black list
 - Only open files which you know are "safe" (jpg, png, txt, pdf...)
- Need to open dangerous document?
 - Be extra cautious with verifying the sender identity and trustworthiness

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Defense?

- What about Office documents? Don't activate macros, whatever the document might say
 - Crooks will entice you to do so with fake motives

![Macro virus](http://i.imgur.com/9r91gZE.jpg)

---
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

## Everything is safer on mac

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="dim" -->

> You can then safely open "cute-kitty.jpg "

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

...right?

![Innocuous jpg image](http://i.imgur.com/MlDuWLF.png)

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

...oops


![Boom](http://i.imgur.com/Ilsgobq.png)

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

".jpg<*space*>", not ".jpg"

![Please note the space](http://i.imgur.com/eR1l024.jpg)

Unknown? Executable ? Let's open it with Terminal!

Note:
I learned this neat little trick from a malware researcher. On mac you can have extension with spaces.. therefore .jpg< space > is totally legit, and invisible to the naked eye. What happens when a file with an unknown extension is executable? It defaults to opening it with the terminal!

It is then very easy to hide the thing by displaying a fake jpg icon and opening a decoy image upon launch.
___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Defense?

- Right-click > Properties on Windows
 - Also configure it to always show known extensions
- Cmd+I or Right-click > Get Info on Mac
 - Preview function can help a lot too

---
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dimblur shadow"-->

# The "Green padlock"

> There is the green padlock, I'm safe then, right?

___
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## The green padlock

What do you think of this website?

![Fake https](http://i.imgur.com/2ax4cGt.jpg)

___
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## The green padlock

 ...woops

 ![Fake https2](http://i.imgur.com/KVeh0Wz.jpg)

___

<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## HTTPS true meaning

- The green padlock only means one thing
 - The communication between your computer and the website is encrypted...
 - ...and the certificate used for the encryption have been proved to be legit...
 - ...for *THIS* domain
- That's all.

___

<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## HTTPS is everywhere

- Getting a recognized certificated used to be long and costly
 - Now, it's free and takes less than 5 minutes
 - Phishing website use HTTPS to look trustworthy

![Fake https2](http://i.imgur.com/FAE4w5N.jpg)

---
<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dimblur shadow"-->

## The line of death

 > Beyond this line, you can't trust anything


![The line of death](http://i.imgur.com/82ksnzo.jpg)

___

<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

## The line of death

Even above this line, trustworthiness is...relative

![Line of death 2](http://i.imgur.com/wP6Pixl.jpg)


___
<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

What do you think of this website?

![picture in picture](http://i.imgur.com/GHcstCo.jpg)

___
<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

## Metro/ModernUI

...It's even worse...

![metro fullscreen](http://i.imgur.com/9UkAOQv.jpg)

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## Défense?

 - Stick with regular browsers and avoid the ModernUI/Metro one
 - In doubt, try to move the window

---
<!-- .slide: data-background="http://i.imgur.com/TVqYFqF.jpg" data-state="dimblur shadow"-->

## Tabnapping

If your browser often looks like mine, you're in trouble

<!-- .slide: data-background="http://imgur.com/NS6nXlC.jpg" -->

![Please note the space](http://i.imgur.com/sKKKrYr.jpg)

___
<!-- .slide: data-background="http://i.imgur.com/xUlJCOB.jpg" data-state="shadow"-->

## Demo time!

Backup video on youtube: https://www.youtube.com/embed/97kduHI2OGk

___
<!-- .slide: data-background="http://i.imgur.com/xUlJCOB.jpg" data-state="shadow"-->
## Demo video
<video preload="auto" data-audio-controls src="http://www.comptoirsecu.fr/morgan/phishing-advanced/video/tabnapping_example.mp4" width="800" height="600">
</video>

___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## How can I defend against such madness?

- Look at the URL before logging in
- Password managers help a lot
 - They won't autocomplete if it's not the right website

<!-- .slide: data-background="http://imgur.com/LTn9gKy.jpg" -->
---
<!-- .slide: data-background="http://i.imgur.com/hlbHFNH.jpg" data-state="dim" -->

## Ok, that's enough for today

---
<!-- .slide: data-background="http://i.imgur.com/REanWBz.jpg" data-state="shadow" -->

## Any Questions?
