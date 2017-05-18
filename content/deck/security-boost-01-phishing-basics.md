+++
title = "Security Boost #01 - 5 things you thought you knew about phishing!"
type="slide"
theme = "kindred"
lang="en"
summary = "And you thought you knew everything about phishing? Let me show you 5 false assumption about how to spot what is a phish and what is not!"
+++

<!-- .slide: data-background="../pics/bg/hook.jpg" data-state="blur" -->

# 5 things you thought you knew about phishing

### Security Boost #01

*Morgan Hotonnier - Group Security*

> <*f*> for fullscreen, <*space*> for next slide
---
<!-- .slide: data-background="../pics/bg/kahoot.png"  data-state="dim" -->

## Quiz incoming!


___
<!-- .slide: data-background="../pics/bg/kahoot.png"  data-state="megadimblur" -->
## Prepare for the quiz

- Short quiz at the end of this presentation
 - Need a smartphone to participate
 - Participant with highest score gets a prize ;).
- Go to http://kahoot.it and type the code
 - Try it now, it takes time to setup.
---
<!-- .slide: data-background="../pics/bg/hook.jpg"  data-state="dim" -->

## Basic reminder: Phishwhat?

- Phishing: Technique to **manipulate** you into
 - revealing sensitive information
 - installing a malware
 - sending money
 - all of the above

---
<!-- .slide: data-background="../pics/bg/phishing.jpg"  data-state="dimblur" -->

## Phishing "levels"

- Classic (generic)
- **Spear phishing**
- **Whaling**

___
<!-- .slide: data-background="../pics/bg/spearphishing.jpg" data-state="dimblur" -->

## Spear phishing

- Tailored to specific individuals or groups
- Uses details from social medias, previous hacks...

![Faktura fran Telia](../pics/faktura-telia.png)

___
<!-- .slide: data-background="../pics/bg/whaling.jpg" data-state="dimblur" -->

## Whaling


- Targets "big" victims (important or wealthy)
 - CEO, CFO, etc
- Uses detailed personal information and corporate lingo

![Whaling Example](../pics/whaling-ex.jpg)

---

<!-- .slide: data-background-color="#B40404" -->

## Top false assumptions

---
<!-- .slide: data-background-color="#DF7401" -->
## 1. The email sender is the right one, I'm safe!

___

<!-- .slide: data-background="../pics/bg/mailbox.jpg" data-state="dimblur" -->

Spoofing email is doable

![brendan fake](../pics/brendan-fake-mail.png)

Anti-spam solutions usually catch it...usually.

___
<!-- .slide: data-background="../pics/bg/mailbox.jpg" data-state="dimblur" -->

## Email Hijack

If your friend got hacked

![friend hacked](../pics/phishing-hacked-account.jpg)

attacker doesn't even need to spoof anything

___
<!-- .slide: data-background="../pics/bg/magnifying-glass.jpg" data-state="dimblur" -->

## When in doubt, Cross-check

- Preferably on another channel
 - Ex: doubt on an email sent by a friend? Ask them by chat/phone





---
<!-- .slide: data-background-color="#8000FF" -->
## 2. Phishing is only done over email!

___

## It's not just about emails!

- Vishing
- Smishing
- Social media

___
<!-- .slide: data-background="../pics/bg/vishing.jpg" data-state="dim"-->

## Vishing

- Phishing by phone, more expensive for the attacker
  - But greater conversion rate :)
- They have call centers dedicated to this kind of scam
- Don't trust the CallerID, it can be faked

![IRS scam](../pics/irs-scam.jpg)

___

<!-- .slide: data-background="../pics/bg/smishing.jpg" data-state="megadimblur" -->

## Smishing

- Phishing over SMS

![wells faergo smishing](../pics/wells-fargo-smishing.jpg)

Note:

This one is very clever as it tricks the user into thinking they know their credit card number. Let me show you something. Who here has a credit card from a SEB bank account? I bet your card starts with 455262.

Nordea? If it's a debit card it's probably 4539, 4910 or 4918

Those numbers are what we call BIN, or Bank Identification Number, they are not tied to you, they are tied to your bank.

___

<!-- .slide: data-background="../pics/bg/social-networks.jpg" data-state="megadimblur" -->

## Social Network phishing

- Masquerading as the social Network
- Use "infected" friends to make you click on malicious links
- Catphishing to lure you into giving out personal details

![FB phishing link](../pics/fb-phishing-what-are-you-doing-lol.png)






---
<!-- .slide: data-background-color="#31B404" -->
## 3. The website has the green padlock, I'm safe!

___
<!-- .slide: data-background="../pics/bg/green-padlock.jpg" data-state="dimblur"-->

## The green padlock

What do you think of those websites?

![Fake https2](../pics/fake-https-paypal.jpg)

___
<!-- .slide: data-background="../pics/bg/green-padlock.jpg" data-state="dimblur"-->

## The green padlock

 ...woops

 ![Fake https2](../pics/fake-https-2.jpg)

___

<!-- .slide: data-background="../pics/bg/green-padlock.jpg" data-state="dimblur"-->

## HTTPS true meaning

- The green padlock only means one thing
 - The communication is encrypted...
 - ...by a certificate known to be legit...
 - ...for **THIS** domain
- That's all.




---
<!-- .slide: data-background-color="#045FB4" -->
## 4. If the address is the right one, then I'm safe!


___
<!-- .slide: data-background="../pics/bg/typewriter.jpg" data-state="megadimblur" -->
## Typosquatting

> Please visit <span class="fragment highlight-red">rn</span>icrosoft.com for more details

> Sorry, I meant  mi<span class="fragment highlight-red">rc</span>osoft.com

> Damn! I meant micr<span class="fragment highlight-red">p</span>soft.com

![big thumb](../pics/big-thumb.jpg)

Note:
Finally, if they just want you to go there by yourself, they can try to squat common typing mistake.

___
<!-- .slide: data-background="../pics/bg/letters.jpg" data-state="dimblur" -->

## Homographs

Wikip<span class="fragment highlight-red" data-fragment-index="1">e</span>di<span class="fragment highlight-green" data-fragment-index="2">a</span> != Wikip<span class="fragment highlight-red" data-fragment-index="1">&#1077;</span>di<span class="fragment highlight-green" data-fragment-index="2">&#1072;</span>

Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="../pics/bg/letters.jpg" data-state="dimblur" -->

## Homographs

Let's put them next to one another

- <font color="green">e</font><font color="red">&#1077;</font>
- <font color="green">a</font><font color="red">&#1072;</font>


Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="../pics/bg/letters.jpg" data-state="dimblur" -->

## How can I seriously spot that?!

- Thanksfully browsers got your back
 - Link are displayed in **punycode**
 - This makes a text like this : http://www.pa&#1091;pal.com
 - Look like this: http://www.xn--pypal-4ve.com/

![Punycode example](../pics/punycode-example.png)

...but
___
<!-- .slide: data-background="../pics/bg/letters.jpg" data-state="dimblur" -->

## Punycode is not perfect

- Doesn't trigger if full domain name uses foreign alphabet
 - The result can be pretty scary
 - What about buying a new iPhone on https://аррӏе.com

 ![Punycode apple](../pics/punycode-apple.png)

___
<!-- .slide: data-background="../pics/bg/letters.jpg" data-state="dimblur" -->
## We're doomed!

 - It's pretty rare though..
 - Password managers to the rescue!

Note:
You can also look at the certificate Common Name, which will always be in Punycode
On firefox you can ask him to always use Punycode, which has basically no downside if you use the latin alphabet.
---
<!-- .slide: data-background-color="#FFF056" -->
## 5. I'm using 2FA, I'm phishing free!

___
<!-- .slide: data-background="../pics/bg/2fa.jpg" data-state="dimblur" -->

## 2FA is great, not bullet proof

- 2FA can be bypassed
 - Website vulnerability
 - Social engineering
 - OAuth

___

## OAuth Phishing Example : Google Docs
<iframe width="560" height="315" src="https://www.youtube.com/embed/rGI3zvl53u0?rel=0" frameborder="0" allowfullscreen></iframe>

___

## Bypassing 2FA : EvilGinx

<iframe width="560" height="315" src="https://www.youtube.com/embed/srieYiogbxk?rel=0" frameborder="0" allowfullscreen></iframe>

---
<!-- .slide: data-background="../pics/bg/sleepy-cat.jpg" data-state="dim" -->

## Ok, that's enough for today

---
<!-- .slide: data-background="../pics/bg/questions.jpg" data-state="shadow" -->

## Any Questions?

---
<!-- .slide: data-background="../pics/bg/kahoot.png"  data-state="dim" -->

## Quiz Time!

http://kahoot.it
