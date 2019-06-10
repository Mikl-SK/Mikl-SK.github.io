---
layout: post
title: Placement Ghost
subtitle: spil
---

Vi har lavet et placement ghost object, som med fx vores drill viser drillen på spillerens cursor inden den bliver sat, samt viser en rød
drill der hvor den ikke kan sættes. Placement ghost viser også prisen på hvad end spilleren har highlightet, hvis den ting man vil sætte,
har en pris.
Vi har lavet det her fordi, vi syntes det ville være rart for spilleren at have en ekstra indikator til hvad det er man er ved at bygge.
Og så er det også rart at vide hvor man ikke kan bygge tingene henne.

I create eventet har vi koden til standarten når objectet bliver kaldt. Det vil sige at der ikke er noget som er highlightet endnu,
og derfor skal der ikke vises noget ghost ej heller nogen pris.

Her ses koden til placement ghost [create event](https://drive.google.com/file/d/1XwwMflecEMn5o73mKnTBw5avuuk_BjTl/view?usp=sharing)

I step eventet, har vi koden som bestemmer hvad der sker når den individuelle maskine er highlightet.

[step event](https://drive.google.com/file/d/1bFeWhWxm11pMWKTkilP2v5ppLnPY49SR/view?usp=sharing)

I glob left released checker vi om der er noget i vejen for at en maskine kan blive placeret, og hvis det ikke er tilfældet bliver maskine
sat.

[glob left released](https://drive.google.com/file/d/1T_2mNsxcVsNJZhKADvq5Ka9BW1e1nNEN/view?usp=sharing)

I draw eventet, bliver spriten som hører til den maskine spilleren har highlightet, tegnet oven på cursoren sammen med den pris om høre
dertil

[draw event](https://drive.google.com/file/d/18-Tu_FAvTI8Y-cjDIkMDXRmzwjebdPjc/view?usp=sharing)
