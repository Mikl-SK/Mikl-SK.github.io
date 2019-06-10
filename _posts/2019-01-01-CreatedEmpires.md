---
layout: post
title: Empires
subtitle: spil
---

Vi har tilføjet nogle 3 forskellige empires til spillet. Lige nu er Danmark, Fyn og Jylland blevet tilføjet som empires (meget kreative navne). Ideen med at have flere empires er at det skal have en betydning for historien, hvilke empires som spilleren vælger at sælge til og så vi har også snakket om at spilleren får mulighed for at vælge et empire frem for et andet, i forbindelse med krig. Det med at vælge et empire i forbindelse med krig, er ikke noget som vi har implementeret endnu, og det skylde at spillet lige nu ikke har nogen historie. Dog har vi tilføjet events og andre former for ændring som der kan forekomme for 1 eller flere empires, mens der bliver spillet.

Der vises kun billeder for empire1Controller, da koden for de 2 andre er mere eller mindre den samme, dog med forskellige værdier.

I create eventet sætter vi nogle standart værdier for priser, navn, affinity og war. Lige nu er det kun priserne som faktisk bliver brugt. De andre værdier er her fordi vi har eksperimenteret med kode tilhørende de ting som lige nu ikke er en del af spiller, som der snakkes om lidt længere oppe i posten.

Her ses koden til empire1Controller [create event](https://drive.google.com/file/d/1Dt5dsoWj-t5q532w7AHLYl9PvZVUSz0b/view?usp=sharing)


Derudover har vi lavet en empireSelector som vi bruger til at vælge empire i sales terminal.

I step eventet har vi koden som viser hvilket empire som der er valgt i sales terminal menuen, hvis den altså eksistere, hvis ikke spawner de uden for skærmen. Grunden hertil kan der læses mere om i posten om sales terminal.

[step event](https://drive.google.com/file/d/148XLrdY21ZoertFJVtLBhjCOJaeXvF3n/view?usp=sharing)

I left released eventet har vi koden som vi bruger til at skifte mellem empires.

[left released](https://drive.google.com/file/d/1AaVCevb9olYXcDjUqJv0oaVI0tzfTMMC/view?usp=sharing)
