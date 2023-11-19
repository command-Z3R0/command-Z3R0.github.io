---
layout: single
title: Les attaques de type HID
excerpt: "Comment s'introduire dans un ordinateur avec des périphériques amovibles, en utilisant des méthodes simples et du matériel accessible"
date: 2023-07-13
classes: wide
header:
  teaser: /assets/images/HID/ducky.png
  teaser_home_page: true
  icon: /assets/images/ducky.webp
categories:
  - Hardware
  - Fait-maison
tags:
  - HID
  - Hacking
  - Payload
  - Bad-usb
  - Rucky

---

<p align="center">
<img src="/assets/images/HID/HID.jpg" width="500">
</p>

Les attaques **HID** (*Human Interface Device*) constituent un moyen étonnamment furtif de pénétrer la sécurité informatique. Ces attaques exploitent des périphériques USB apparemment inoffensifs, tels que des claviers et des souris, pour effectuer des actions malveillantes de manière discrète. Dans cet article, nous explorons le monde obscur des attaques HID, en découvrant comment ces dispositifs apparemment ordinaires peuvent devenir des outils puissants pour les pirates et les cybercriminels. Découvrez comment ces attaques sont exécutées et les vulnérabilités qu'elles exploitent - préparez-vous à plonger dans le monde intrigant de la cybersécurité et à comprendre comment les attaques HID redéfinissent le paysage des cybermenaces ! 


# Explorer la subtilité de l'intrusion avec des périphériques USB.
__________________________________________________________________________________________________________________________________

Dans le monde intrigant de la cybersécurité, les attaques par dispositifs d'interface humaine (HID) se distinguent par leur furtivité et leur capacité à échapper aux défenses conventionnelles. Ces attaques tirent parti de l'apparente innocence des périphériques USB courants, tels que les claviers et les souris, pour s'infiltrer dans les systèmes de manière furtive et souvent imperceptible.


## Comment fonctionnent-ils ?

Les attaques HID reposent sur la capacité de ces dispositifs à émuler la fonctionnalité d'un clavier ou d'une souris. Lorsqu'ils sont connectés à un ordinateur, ces périphériques peuvent envoyer des commandes automatiques qui imitent les actions d'un utilisateur légitime. Qu'il s'agisse d'exécuter des scripts, d'ouvrir des programmes ou de manipuler des paramètres, les attaques HID exploitent l'apparence inoffensive de ces périphériques pour effectuer des actions malveillantes sans éveiller les soupçons.

## Scénarios d'attaque :

**Injection de commande :**
- Les attaquants peuvent programmer des scripts qui, lorsqu'ils sont exécutés par l'intermédiaire d'un dispositif HID, introduisent un code malveillant dans le système, en exploitant les vulnérabilités existantes.

**Reconnaissance et exfiltration des données :**
- En utilisant des scripts spécifiques, les attaquants peuvent collecter des informations à partir du système et les envoyer à des sites externes, compromettant ainsi la confidentialité des données sensibles.

**Élévation des privilèges :**
- Les attaques HID peuvent être utilisées pour modifier la configuration du système, ce qui permet une escalade des privilèges et donne aux intrus un plus grand contrôle sur la machine compromise.

## Exemple pour comprendre le potentiel de cette attaque.
<iframe width="480" height="270" src="https://www.youtube.com/embed/XW6f86LXQ2I" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Comment mener cette attaque ?

Cette attaque nécessite un dispositif capable de simuler un clavier ou une souris. L'entreprise <a href="https://hak5.org/" target="_blank">Hak5</a> a le dispositif appelé <a href="https://hak5.org/collections/best-selling/products/usb-rubber-ducky" target="_blank">Rubber Ducky</a> qui est commercialisé et accessible au public, mais dont le prix est assez élevé, et que nous écartons donc aujourd'hui.

Il s'agit des appareils les plus couramment utilisés pour mener cette attaque :

 - Arduino uno

<p align="center">
<img src="/assets/images/HID/arduno.png" width="270">
</p>
 

 - Digispark
 
 <p align="center">
<img src="/assets/images/HID/digi.png" width="270">
</p>
 
 - CJMCU microSD
 
<p align="center">
<img src="/assets/images/HID/cjmcu.jpg" width="270">
</p> 


 - Un smartphone avec les privilèges de l'administrateur (root)

<p align="center">
<img src="/assets/images/HID/rootphone.png" width="270">
</p>


__________________________________________________________________________________________________________________________________


Dans le prochain article, nous verrons comment créer un bad-usb.




    





