---
title: "Hello World!"
date: 2018-04-28T23:23:18+02:00
draft: true
---

Úplne prvý článok na novom blogu. Lepšie povedané na úplne novom systéme. 2 roky som bol na wordpresse, nedá sa povedať že som bol nespokojný, skôr mi to prišlo ako príliš **"heavy"** systém na tie moje 3 články. Taktiež som chcel niečo viacej lightweight. Mal som na obzore pár systémov ako napr [Grav](https://getgrav.org/) alebo [Jekyll](https://jekyllrb.com/) a taktiež som skúsil aj od českých bratov [Statie](https://github.com/Symplify/Statie). Ako si si mohol všimnúť všetko sú to static site generátory. To som presne chcel. Niečo malé, nenásilné. Nemám problém napísať markdown súbor, pushnúť to na github a potom pullnúť na server. Pretože websupport moc možností nemá. Čo je tak trošku narážka na websupport? Debaty hodné.

## Chcel som aj Ghost lenže...
Na obzore bol aj ghost. CMS systém ktorý sa mi veľmi páči. Napísaný v **node.js**, rýchly, svižný. Používali sme ho v [thinkapple](https://www.thinkapple.sk/), takže som vedel čo od neho očakávať. Taktiež má prístupné super témy a hlavne pomocou **JavaScriptu** sa tam dajú doplniť pluginy podľa vlastného vkusu. Sám si dokódiš. Úplne sám. Tak som zobral svoj voľný čas. Konkrétne tých 5 minúť denne 😂 nainštaloval si ghost lokálne, všetko nastavil a ide sa na websupport hosting. `git clone`, `cd blog`, `node -v`, wait what? Síce je na chválu, že websupport má najnovší node na serveroch, lenže ghost potrebuje LTS verziu, čo nieje vždy najnovšia verzia. Teda.. skoro nikdy. Musíš fakt vychytať dátum kedy releasnu LTS verziu, potom máš pár dní najnovší node, aj LTS verziu. Takže hopy šupky na support chat. Chvalabohu tam majú tak úžasných ľudí ako majú 😉, ale to môj problém nevyriešilo. Dal sa riešiť jedine kúpou VPS serveru, čo v mojom prípade nebolo riešenie nakoľko vlastný server fakt nepotrebujem. Ghost ako taký ponúka vlastný server za $20/month, čo je ešte drahšie ako najlacnejšie VPS. Takže som musel nájsť niečo iné.

## Náhodou som natrafil na huga
Náhodou som niečo hľadal na nete. Narazil som na blog jedného poľského developera. Hneď som to hodil do [Built With](https://builtwith.com/). Zistil som, že tam je nejaký HUGO. Tak som si pogooglil viacej. Hugo je tiež Static site generator. Ale postavený na GOlangu. Čo dúfam že na hosting nahodím. Čiže ak toto čítaš tak som to úspešne nahodil. Chvalabohu.   
Ide o to, že ak to nahodíš na svoj OS, príde ti pred-kompilovaný systém. Ty si nahodíš všetko a potom to len **deployneš?**. Nechcem to zakríknuť.  
*Edit: nakoniec som to musel hodiť na github. Asi som moc vyberavý.*🙃
  
Nakoľko je hugo napísaný v golangu, je to dosť rýchly systém. Je to easy to use fakt mi to zabralo pár príkazov
```
$ brew install hugo
$ hugo new site website
$ cd website
$ git clone https://github.com/luizdepra/hugo-coder.git themes/coder
$ echo 'theme = "coder"' >> config.toml
$ hugo new posts/prvy-post.md
```

**BUM** Máš web ako ja. Potom ešte samozrejme to trošku nakonfigurovať. Viacej o tom nájdeš v repozitári svojej témy, čo sa tej mojej týka [nájdeš to tu](https://github.com/luizdepra/hugo-coder). Nezabúdaj, že inštalácia je rozdielna na rôznych operačných systémoch, takže na HugoDocs sa dozvieš [viac](https://gohugo.io/getting-started/quick-start/). Uvidíme ako budem spokojný ale so far so good.
