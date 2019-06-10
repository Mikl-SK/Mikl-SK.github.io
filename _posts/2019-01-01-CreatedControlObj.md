---
layout: post
title: Control object
subtitle: spil
---

Vi har lavet et control object, som indeholder en masse globale variabler, vores cycle, den styrer hvad der sker når man ruller med
midterste musse knap og så tegner den vores UI. De globale variabler som den indeholder, er variabler som vi tilgår og ændre i, i flere
af vores objecter fx priserne på recourser. Når det er vi bruger de samme variabler så mange forskellige steder, er det nemmere at have
dem samlet et sted. 

I create eventet har vi alle vores globale variabler. Det er også her vores spiller instance bliver lavet.

Her ses koden til control [create event](https://drive.google.com/file/d/1imBZVIjgm-ZubDpT9xuUbbuxmOLEoqLY/view?usp=sharing)

Alarm 0 er vores cycle timer.

[alarm 0](https://drive.google.com/file/d/1smzbICprymgXjmrmEyYb5w02wdrBwvHV/view?usp=sharing)

I step eventet, kører vores events samt vores upkeep, når en cycle ender.

[step event 1. del](https://drive.google.com/file/d/1SHqsUrt7xuFpb2FXLPxKlP_T_29uGnj-/view?usp=sharing)

[step event 2. del](https://drive.google.com/file/d/1-yiFUrnvqthWOaV3M_LRQhY-W3H04FXz/view?usp=sharing)

Mouse wheel up og down, er koden som flytter på den highlightet boks på UI i bunden af skærmen, som indikere hvilken maskine du har valgt

[mouse wheel up](https://drive.google.com/file/d/1cnd9gB3la9gP2CZFGdPbdB9i8FObv_II/view?usp=sharing)

[mouse wheel down](https://drive.google.com/file/d/1mpek2hqKYO4YF5jVPxos3bn6L0hFLFqW/view?usp=sharing)

Draw GUI tegner vores UI.

[draw GUI](https://drive.google.com/file/d/1Bj8zeR-XjmxhVIaG_9yk_x0yZIUabHnU/view?usp=sharing)
