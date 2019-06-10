---
layout: post
title: Sales terminal
subtitle: spil
---

Vi har lavet en sales terminal, som er en maskine som spilleren kan placere og som bruges til at sælge de recourser som spilleren har
samlet. Spilleren kan vælge ved brug af en pil i bunden af menuen, hvilket empire vedkommende har lyst til at sælge til. Lige nu sker der
ikke noget ved at spilleren sælger til et bestem empire. Men vi har snakket om at det på et tidspunkt skulle have en betydning.
Hvis spilleren sælger meget af en bestemt recourse på en gang, vil prisen for den bestemte recourse falde mere og mere, ned til et bestemt
punkt. Dette er et forsøg på at simulere noget intelligens i forhold til salg.
Vi har også nogle events som kan ske efter hver cycle ender(det kan der læses mere om i even posten). Dette kan have en effekt på priserne,
og her er det smart at spilleren kan skifte mellem empires, da events kun rammer nogle bestemte empires. Så hvis priserne er lave et sted,
så kan de være højere et andet sted.

Knapperne i menuen bliver spawnet oven på menuen. På den måde har vi lidt mere frihed til at give knapperne deres egen sprite.

Der vises kun billeder for sellMin knappen, da koden for alle knapperne er den samme, dog med andre værdier.

I create eventet sætter vi en standart værdi for mængden af penge som spilleren skal modtage, dette ændres alt efter recourse, events og
empire. Derudover har vi en variable som tjekker hvilket empire som er valgt.

Her ses koden til sellMin knappen [create event](https://drive.google.com/file/d/1YGmYB_mGJtBW0dLtvCrRnF6KkzaSfX-C/view?usp=sharing)

I step eventet bliver knapperne placeret på menuen, hvis altså menuen existerer, hvis ikke den eksistere bliver knapper lavet uden for
skærmen. Vi gør det på denne måde fordi, siden vi har lavet knapperne som deres egne objecter så er vi nødt til at skal ligge dem ind i
det room hvor de skal bruges. Og siden de skal kunne ses af spilleren, så kommer de til at kunne ses lige meget hvad. Derfor spawner vi
knapperne uden for skærmen når det er de ikke bruges.

[step event](https://drive.google.com/file/d/1hS3Jebn0wRo1mrTvkvcH67XGr2p5Egdr/view?usp=sharing)

I left released eventet har vi koden som afgører hvad der sker når spilleren trykker på knapperne.

[left released](https://drive.google.com/file/d/1X15ukLMZzfCBr8o6AE4LXtvGx8rHKKDJ/view?usp=sharing)
