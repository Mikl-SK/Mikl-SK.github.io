---
latout: post
title: Recourses
subtitle: spil
---

Vi har lavet recourser til vores spil. Lige nu er der 3 forskellige recourser, minerals, valuables og fuel. Hver recourse er deres eget
object, men fungere afhængigt af drill og så en recourse node.
Vi har sat det op på den måde at, der spawner forskellige recourse nodes på banen, 3 nodes specifik, 1 til hver. Når der så placeres en
drill oven på en af de nodes, spawner drillen recourser alt efter hvilken node den er placeret på. Recourserne spawner med forskellige
hastigheder, fordi de har forskellige værdier plus at mængden af recourse nodes og så variere alt efter hvilken node der er tale om.
Valuables er den recourse som er mest værd, og er derfor også den recourse som har færrest nodes, og der er også den recourse som drillen
spawner langsomst.

Der bliver kun vist billeder for valuables, og det er fordi koden er den samme for alle recourser, dog med forskellige værdier.

I create eventet, bliver der valgt en tilfældig retning som recoursen flyver i, når den bliver spawnet samt hvor langt den kan flyve væk.
Det er også her vi vælger hvor hurtigt den kan blive spawnet.

Her ses koden til valuables [create event](https://drive.google.com/file/d/1PI4inhztifZ0hltpqIp0eKPswR5PaUoI/view?usp=sharing)

I alarm 0 har vi koden som får recoursen til at stoppe, alt efter hvilken range der er blevet valgt tilfældigt mellem 5 og 10.

[alarm 0](https://drive.google.com/file/d/1B59y-BsbYdbX_zP5Uid8OjNt8ctSdG98/view?usp=sharing)

I alarm 1 har vi koden til hvor hurtigt en recourse skal flyve mod spilleren eller storage, givet spilleren eller storage er tæt nok på.

[alarm 1](https://drive.google.com/file/d/1G9QA5xjloxRwVBob7qoqLNoqHDlEFrFH/view?usp=sharing)

I step eventet har vi koden, som afgøre om spilleren eller storage er tæt nok på til at recoursen skal flyve mod dem.

[step event](https://drive.google.com/file/d/1e1Ng10fW79XlTt4YX79F17ynrfp83KPO/view?usp=sharing)

I player eventet har vi koden som hvis spilleren samler recoursen op, øger mængden af valuables i spilleren inventory, hvorefter den
destruerer sig selv.

[player event](https://drive.google.com/file/d/161mKpA7370dpUpM0v2WUqwzTxUr9c4JA/view?usp=sharing)

I valuables storage eventet har vi den samme kode som i spiller eventet, men bare for storage istedet.

[storage event](https://drive.google.com/file/d/13QN-bPS124S6Az-mWSSy--CwHBXG_pzv/view?usp=sharing)
