+++
title = "Techniques de phishing avancées"
type="slide"
theme = "kindred"
lang="fr"
+++
<!-- .slide: data-background="http://i.imgur.com/iXrdLRm.jpg" data-state="blur shadow" -->

# Techniques de phishing avancées

### Et comment s'en protéger

*Morgan Hotonnier - Group Security*

> <*f*> pour mettre en plein écran, <br /> <*espace*> pour continuer

---
<!-- .slide: data-background="http://i.imgur.com/iXrdLRm.jpg" data-state="dim" -->

## Techniques avancées

- Email Hijacking
- Typosquatting
- Homographes
- Technique "RTL"
- Redirections et raccourcis
- Extensions de fichier
- Pièces jointes dangereuses
- Https = sécurisé?
- La ligne maginot
- Tabnapping

---
<!-- .slide: data-background="http://i.imgur.com/0V1Gtro.jpg" data-state="dim" -->

## Email Hijacking

Si un ami/collègue se fait pirater

![friend hacked](http://imgur.com/qp1GiCG.jpg)

L'attaquant n'a même plus besoin d'utiliser des techniques de spoofing

---
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="shadow blur" -->

## Typosquatting

> Visitez <span class="fragment highlight-red">rn</span>icrosoft.com pour plus de détails

note:

Sometimes it is very difficult to differentiate visually some letters, or groups of letters, from others, typosquatteur will use it to make their phishing link looks legit
___
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="dim" -->

## Typosquatting

> Pardon, je voulais dire  mi<span class="fragment highlight-red">rc</span>osoft.com

<iframe src="https://geon.github.io/programming/2016/03/03/dsxyliea" width="800" height="400"></iframe>

Note:

Another easy way is to invert two letters in the url, if you don't look carefully you may not even notice it
___
<!-- .slide: data-background="http://i.imgur.com/bJ3qul1.jpg" data-state="dim" -->
## Typosquatting

> Décidemment! je voulais bien sûr taper micr<span class="fragment highlight-red">p</span>soft.com

![big thumb](https://cdn.meme.am/instances/39718882.jpg)

Note:
Finally, if they just want you to go there by yourself, they can try to squat common typing mistake.

---
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## Homographes

Wikip<span class="fragment highlight-red" data-fragment-index="1">e</span>di<span class="fragment highlight-green" data-fragment-index="2">a</span> != Wikip<span class="fragment highlight-red" data-fragment-index="1">&#1077;</span>di<span class="fragment highlight-green" data-fragment-index="2">&#1072;</span>

Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## Homographes

Regardons ça de plus prêt

- <font color="green">e</font><font color="red">&#1077;</font>
- <font color="green">a</font><font color="red">&#1072;</font>


Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
___
<!-- .slide: data-background="http://i.imgur.com/7Pm537O.jpg" data-state="dimblur" -->

## Comment je repère ça à l'oeil nu moi?!

- Heureusement, les navigateurs sont là pour nous aider
 - Les liens sont toujours affiché en **punycode**
 - Cela signifie qu'un lien comme celui-ci : http://www.pa&#1091;pal.com
 - Sera affiché de cette manière: http://www.xn--pypal-4ve.com/

![Punycode example](http://i.imgur.com/dxSJqSX.png)


Note:
https://en.wikipedia.org/wiki/IDN_homograph_attack
---
<!-- .slide: data-background="http://i.imgur.com/21XrAzX.jpg" data-state="dim" -->

## Technique RTL

> etiord à ehcuag ed suot sap snosil en suon euq ecraP

note:
http://www.rafayhackingarticles.net/2016/08/google-chrome-firefox-address-bar.html?m=1
___
<!-- .slide: data-background="http://i.imgur.com/21XrAzX.jpg" data-state="dim" -->

### Technique RTL

Le lien http://عربي.امارات/google.com/test/test/test était affiché de cette façon

![RTL Attack](http://i.imgur.com/sR2cLnN.png)

C'est patché...<span class="fragment highlight-red">pour l'instant</span>.

note:
http://www.rafayhackingarticles.net/2016/08/google-chrome-firefox-address-bar.html?m=1

---
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="shadow" -->

### Redirections

___
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="dim" -->

## Mini-liens

> Parce que http://tiny.cc/recover-gmail-password inspire confiance, n'est ce pas?

___
<!-- .slide: data-background="http://i.imgur.com/dWzjeiz.jpg" data-state="dim" -->

## Redirections ouvertes

Que dites vous de ce lien là? <a href="#">http://www.ebay.com/longue/url/legitime/<span class="fragment highlight-green">redirection.php?url=http://malicious.example.com</span></a>

Note:
Peut aussi être réalisé en Javascript sur un site vulnérable (XSS)
___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## Défense?

Vous pourriez tout simplement cliquer sur le lien et voir ou cela fini par vous ammener...

...mais si la destination exploite une vulnérabilité de votre navigateur/plugin flash/pdf...

vous pourriez être infecté rien qu'en affichant la page.

___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

Il existe aussi des "expanders" http://www.linkexpander.com/

![link expander example](http://i.imgur.com/ByM4PuW.png)

---
<!-- .slide: data-background="http://i.imgur.com/TVqYFqF.jpg" data-state="dimblur shadow"-->

## Extensions de fichier

> Double-cliquer pour ouvrir photo-coquine.jpg<font color="gray"><span class="fragment highlight-red">.exe</span></font>

![double extension trick](http://i.imgur.com/WX7NY9M.png)

---
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="shadow"-->
## Pieces jointes dangereuses

___
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="dimblur shadow"-->

## Pieces jointes dangereuses

> Ce n'est pas un .exe, je peux donc l'ouvrir sans crainte?

___
<!-- .slide: data-background="http://imgur.com/Y9FGUNm.jpg" data-state="dim"-->

## Pieces jointes dangereuses

- C'est plus compliqué que ça
- Le nombre d'extensions dangereuses dépasse les 50
 - .pif, .msi, .com, .scr, .msc, .jar, .bat, .cmd, .vb, .js, .ps1, .msh, .lnk, .inf, .reg
 - Mais aussi .svg, .doc, .xls, .ppt...

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Défense?

- Préférez le concept de liste blanche à celui de liste noire
 - N'ouvrez que ce que vous savez être sans risque (jpg, png, txt, pdf)
- Document à risque? N'ouvrez que si
 - Vous connaissez l'Expediteur
 - Il vous a confirmé (par un autre canal) que le mail venait bien de lui

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Défense?

- Documents offices? N'activez pas les macros
 - Peu importe ce que dit le document

![Macro virus](http://imgur.com/9r91gZE.jpg)

---
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

## Oui mais sur Mac, on a pas de virus

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="dim" -->

> Vous pouvez donc ouvrir sans crainte "cute-kitty.jpg "

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

...n'est ce pas?

![Innocuous jpg image](http://i.imgur.com/MlDuWLF.png)

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

...oups


![Boom](http://i.imgur.com/Ilsgobq.png)

___
<!-- .slide: data-background="http://i.imgur.com/Q9gF5kV.jpg" data-state="shadow" -->

".jpg<*espace*>", pas ".jpg"

![Please note the space](http://i.imgur.com/eR1l024.jpg)

Extension inconnue? Marqué comme éxecutable ? Ouvrons le donc avec un terminal!

Note:
I learned this neat little trick from a malware researcher. On mac you can have extension with spaces.. therefore .jpg< space > is totally legit, and invisible to the naked eye. What happens when a file with an unknown extension is executable? It defaults to opening it with the terminal!

It is then very easy to hide the thing by displaying a fake jpg icon and opening a decoy image upon launch.
___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

# Défense?

- Clic-droit > Propriétés sur Windows
 - Pensez à configurer l'explorateur pour qu'il affiche les extensions des fichiers dont le type est connu
- Commande+I ou clic-droit > Informations sur Mac
 - La fonction de prévisualisation est aussi pratique (barre d'espace)

---
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dimblur shadow"-->

# Le "Cadenas vert"

> Il y a le petit cadenas, je suis sur un site de confiance

___
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## Le cadenas vert

Que pensez vous de ce site?

![Fake https](http://imgur.com/2ax4cGt.jpg)

___
<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

## Le cadenas vert

...oups

![Fake https2](http://imgur.com/KVeh0Wz.jpg)

___

<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

# Ce que signifie HTTPS

- Le cadenas dans la barre ne signifie qu'une chose
 - La connexion entre votre ordinateur et le site est chiffrée
 - et le certificat utilisée est reconnue par une autorité de certification...
 - ...comme appartenant à ce nom de domaine
- C'est tout.

___

<!-- .slide: data-background="http://imgur.com/QMGytDJ.jpg" data-state="dim"-->

# HTTPS est partout

- Avant, avoir un certificat validé était long et couteux
 - Maintenant, c'est gratuit et ça prend 5 minutes
 - Les faux sites passent en HTTPS pour inspirer confiance

![Fake https2](http://imgur.com/FAE4w5N.jpg)

---
<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dimblur shadow"-->

# La zone de confiance

> Passez cette ligne, rien n'est fiable


![Ligne rouge](http://imgur.com/82ksnzo.jpg)

___

<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

# La zone de confiance

Et même au dessus de cette ligne, tout est relatif...

![Ligne rouge...ou pas](http://imgur.com/wP6Pixl.jpg)


___

<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

Que pensez vous de ce site?

![picture in picture](http://imgur.com/GHcstCo.jpg)

___
<!-- .slide: data-background="http://imgur.com/azkJvLy.jpg" data-state="dim"-->

# Metro/ModernUI

...C'est pire...

![picture in picture](http://imgur.com/9UkAOQv.jpg)

___

<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## Défense?

- N'utilisez pas l'interface Metro de Windows 8/10
- En cas de doute essayez de bouger la fentre

---
<!-- .slide: data-background="http://i.imgur.com/TVqYFqF.jpg" data-state="dimblur shadow"-->

## Tabnapping

Si votre navigateur ressemble souvent au mien, vous êtes dans le pétrin

<!-- .slide: data-background="http://imgur.com/NS6nXlC.jpg" -->

![Please note the space](http://i.imgur.com/sKKKrYr.jpg)

___
<!-- .slide: data-background="http://i.imgur.com/xUlJCOB.jpg" data-state="shadow"-->

## Démonstration!

Vidéo backup: https://www.youtube.com/embed/97kduHI2OGk

___
<!-- .slide: data-background="http://i.imgur.com/xUlJCOB.jpg" data-state="shadow"-->
## Démo vidéo
<video preload="auto" data-audio-controls src="http://www.comptoirsecu.fr/morgan/phishing-advanced/video/tabnapping_example.mp4" width="800" height="600">
</video>

___
<!-- .slide: data-background="http://i.imgur.com/ZJru7gj.jpg" data-state="dim"-->

## Comment se défendre de cette sorcellerie!

- Toujours vérifier la barre d'adresse avant de remplir des données sensibles
  - Pas besoin de cliquer sur entrée, taper dans la fenêtre, c'est déjà trop
- Les gestionnaires de mot de passe aident beaucoup
 - Ils ne feront pas l'autocomplétion vu que ce n'est pas le bon site

---
<!-- .slide: data-background="http://i.imgur.com/hlbHFNH.jpg" data-state="dim" -->

## Ok, ça suffira pour aujourd'hui

---
<!-- .slide: data-background="http://i.imgur.com/REanWBz.jpg" data-state="shadow" -->

## Des questions?
