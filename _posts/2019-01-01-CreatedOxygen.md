---
layout: post
title: Oxygen
subtitle: spil
---

Vi snakkede om i gruppen at vi gerne vil have et oxygen system, som skal være en ekstra ting som spilleren skal holde øje med.
Når spillere ikke længere har noget oxygen tilbage, dør spilleren og det er derfor game over. Måden hvorpå spilleren får mere oxygen,
er ved at købe det ved en oxygen terminal. Spilleren skal derfor sørge for at have nok penge til at købe mere oxygen. Vi tænkte at 
det ville være godt at have noget mere for spilleren at holde øje med, og som ville passe godt ind med det cycle system som der er i
spillet.

Som det ser ud lige nu, så er oxygen terminalen ikke helt færdig. Plus at der ikke sker noget når spilleren rammer 0 oxygen lige nu. 
Dette skylde at vi ikke har implementeret noget "game over" endnu. Vi har ikke i gruppen snakket så meget om game over. Det har været mere
vigtigt for os i gruppen at sørge for at mange af de andre funktioner virker først.

Måden hvorpå oxygen terminalen er lavet på, er ved at have en terminal som kan sætte in-game, som viser en menu når spilleren kommer 
tæt nok på. Selve menuen fungere ligesom nogle af de andre menuer som også kommer frem når spilleren kommer tæt nok på den respektive 
terminal. Der hvor denne menu er lidt anderledes er, hvor vi laver et knap object som vi spawner sammen med menuen når den popper frem.
Så selve menuen viser kun mængden af oxygenen som du har tilbage og hvor meget det koster at købe mere, også tager knap objectet sig af 
at trække penge fra spilleren og give spilleren mere oxygen.

Her ses koden til oxygen button [create event](https://drive.google.com/file/d/1qU3jAmhLIgrjR6Oioy4EsPbqyU38qP_L/view?usp=sharing)

Her ses koden til oxygen button [left released](https://drive.google.com/file/d/1sHU9y7FvRCqji_Y9QP1Twq05qNP5XQ-A/view?usp=sharing)

Her ses koden til oxygen button [step event](https://drive.google.com/file/d/1VyOcfxMoFBRS7_sibRX38iu9_DqJOER4/view?usp=sharing)

Her ses koden til oxygen control[step event](https://drive.google.com/file/d/1mOhfG1q8kXcUyH1kZQlnLJxxzVzuO0Up/view?usp=sharing)

Her ses koden til oxygen terminal[step event](https://drive.google.com/file/d/1On-j1Ear2Bm3y2SbuvryTLxDfN0m5MDU/view?usp=sharing)

Her ses koden til oxygen terminal[draw event](https://drive.google.com/file/d/1eucwX4fCamF3iQsgm0Icrc8fHTy78U6K/view?usp=sharing)

Her ses koden til oxygen terminal[step event](https://drive.google.com/file/d/11jGPT8D0xH8uwBB0uDu0W1qdAJ4APrcd/view?usp=sharing)
