---
layout: post
title: Upgrade menu
subtitle: spil
---

Vi har tilføjet en upgrade menu, som spilleren kan tilgå ved at trykke på U-tasten. I menuen kan der købes forskellige opgraderinger til 
spilleren, turret, drill og maskiner generalt. Vi tænkte det kunne være sjovt at have mulighed for at opgradere sine maskiner mm. undervejs
som man spiller spillet, også i det spillet bliver sværre mens man spiller. Lige nu har spillet den samme sværdhedsgrad hele tiden, og
derfor har opgraderingerne ikke den store betydning lige nu. Lige nu er der heller ikke tilføjet nogen pris for at opgradere, det er 
udelukkende en tidlig version af opgradering.

Ligesom vi har gjort tidligere, så har vi lavet selve knappen som et object for sig selv, som så bliver spawnet ovenpå menuen når den
spawnes.

I create eventet har vi koden som fortæller hvilke værdier topPosX - og y skal have.

[create event](https://drive.google.com/file/d/13ZeQoCCtQuikr4HkjuTCTkOdd8oWUcoN/view?usp=sharing)

I end step eventet har vi koden som spawner knapperne på menuen, når menuen spawnes.

[end step event](https://drive.google.com/file/d/1O3beFjShwAIuzGmwAE-RXDNcPyiVQtRi/view?usp=sharing)

I left released eventet har vi koden som bliver kørt når der trykkes på buy knappen, alt efter hvilken Ypos som knappen har i menuen.

[left released](https://drive.google.com/file/d/1vk4bMQxyLOttQI4duwFuESF1IEu_F0ls/view?usp=sharing)


I menuens create event har vi kode som også spawner knapperne ind, der er lige lidt dobbelt kode her

[create event](https://drive.google.com/file/d/11aHMVLBuhpiGom4vi8LiDyS47BKs0Ntx/view?usp=sharing)

I begin step eventet har vi koden som gør at menuen følger med spilleren, når spilleren bevæger sig samtidig med at menuen er åben.

[begin end step event](https://drive.google.com/file/d/1LsW8EiZLJwKaB1gwxM--H9aAtU7c1Djf/view?usp=sharing)
