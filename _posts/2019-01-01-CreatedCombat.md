---
layout: post
title: Combat
subtitle: spil
---

Vi har lavet noget combat i spillet. Det er ikke det helt store lige nu, men vi skal jo starte et eller andet sted. Vi har tilføjet fjender
som spawner efter hver cycle. Fjenderne vil gå efter nærmeste maskine, turret eller hvis spilleren er tæt nok på tager det prioritet. 
Det her combat er os som forsøger at leje med noget simuleret intelligens, som er en del af vores læringsmål for projektet. Vi forsøger os
med noget simuleret intelligens flere steder, men vi blev enige om at combat ville være en af de bedre måder at vise det på. Spillet er
selvfølgelig stadig i et meget tidligt stadie, og derfor er det ikke super "crazy" lige nu, men det har været fedt og sjovt for os at lege
rundt med.

Det er vores ide at der skal spawne flere og flere fjender, jo flere cycles spilleren har været igennem.


I create eventet sætter vi nogle standart værdier, som mængden af live, hastighed, mængden af skade den giver osv.

Her ses koden til enemy [create event](https://drive.google.com/file/d/1rAlkg11diq5pY9S6guHPxP_9oWOhrkNK/view?usp=sharing)

I alarm 0 har vi kode som vi bruger til at fortælle spillet hvor hurtigt en fjende kan angribe.

[alarm 0](https://drive.google.com/file/d/1ck5EFvGjX200OZlblWMTGfl63Z8EnBJX/view?usp=sharing)

I step eventet har vi koden som alt efter den state som fjenden er i, beskriver hvordan fjenden skal søge, efterfølge, angribe eller 
efterfølge en angriber.

[step event](https://drive.google.com/file/d/1GJweZKJSzuVg3_9XL6V8XnfzmiXskcfE/view?usp=sharing)

I target parent eventet har vi koden som beskriver hvad der sker når en fjende angriber.

[target parent](https://drive.google.com/file/d/1aA97_nqCeLrIKNjJo_tsFQTfrtSaqp-5/view?usp=sharing)


For at kunne forsvare sig, har tilføjet turrets som automatisk skyder efter fjender når de kommer tæt nok på.

I create eventet har vi koden som starter med at lave en turret stand der hvor spilleren placere sin turret. Her fortæller vi også hvor
hurigt den kan skyde, om den kan skyde og hvor meget liv den har.

Her ses koden til turret [create event](https://drive.google.com/file/d/1uMfePtIjk2FaVsklOkgwvVYRwcQtbwbi/view?usp=sharing)

I alarm 0 har vi koden som fungere på præcis samme måde, som koden i alarm 0 i fjende objectet.

[alarm 0](https://drive.google.com/file/d/1U50xLNdi_gaVrfIx4V1l9BFFBLefNomy/view?usp=sharing)

I step eventet har vi koden som fortæller turreten at den skal angribe nærmeste fjende, hvis den eksistere. Derefter kode som fortæller 
om hvorvidt fjenden er tæt nok på, hvis den er så skal turreten skyde.


Til sidst har vi selve skudet som bliver affyret af turreten.

I create eventet har vi koden som fortæller hvor hurtigt skudet skal flyve, og en standart værdi for den fjende som den skal flyve imod.

[create event](https://drive.google.com/file/d/1rvzYSBDmIMjy3LKTf80NHFbs3bKMQbwZ/view?usp=sharing)

I enemy eventet har vi koden som fortæller hvor meget skade skudet skal give til fjende, samt hvilken fjende skudet skal gå efter. Hvor
skudet så til sidst når den rammer en fjende skal desturere sig selv.

[enemy event](https://drive.google.com/file/d/16sZStqOilJECFcD23Uqzv9309LV67tcn/view?usp=sharing)


Her er et billede af hvordan turret of fjende ser ud [in-game](https://drive.google.com/file/d/1FVRV17VBbsAZpBgmoOgONuCladhX5Igj/view?usp=sharing)
