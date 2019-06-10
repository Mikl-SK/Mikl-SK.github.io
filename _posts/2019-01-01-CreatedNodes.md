---
layout: post
title: Nodes
subtitle: spil
---

Vi har lavet recourse nodes og gjort sådan så de spawner tilfældigt på banen, når spillet bliver loadet. Som der også er skrevet i posten
om recouser, så er der 3 forskellige nodes som spawner, minerals, valuables og fuel. Vi bruger nodesne til at indikere hvor på banen
spilleren kan finde udvende disse recourser.
Det var meningen at vi ville gøre sådan så en node forsvinder efter den er blevet udvendet helt, men det har vi ikke kunnet få til at virke.
Det er faktisk noget af de kode som vi har sloges mest med, og som vi ihvertfald for nu har valgt ikke at bruge mere tid på. I forbindelse
med at nodes forsvinder ville vi også have lavet en form for scanner, som skulle hjælpe spilleren med at finde nye nodes. Men det er vi
desværre ikke kommet igang med, da vi ikke har kunnet få noget kode til at virke. Planen var at scanneren skulle "finde"/spawne nye nodes,
men det giver ikke rigtig mening at have en scanner som spawner flere nodes, når det er de gamle nodes stadig er der.

Vi har til nodes lavet et andet object som spawner nodesne på tilfældige steder på banen. Det den gør er at tage en tilfældig x og y værdi,
som er inde for banen og som ikke har nogen instance på sig, og laver en node instance der. Det køre i et "do until" loop, som spawner de
enkelte nodes tilfældige steder indtil det maksimale mængde af de individuelle nodes er ramt.

Her ses koden til spawn node [create event](https://drive.google.com/file/d/1U91eEdagGCC42bWWHL04CoIEWreZ3NoH/view?usp=sharing)


Der bliver kun vist billeder for 1 node, og det er fordi koden er den samme for dem alle sammen, dog med forskellige værdier.

I create eventet har vi koden som beskriver hvilken type recourse det er, og hvor mange drills som er placeret på den.

Her ses koden til [create eventet](https://drive.google.com/file/d/1UpzWdPyIV1SUC648reLHHZFVseZ5ut39/view?usp=sharing)
