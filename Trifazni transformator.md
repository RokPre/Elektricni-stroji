---
related:
  - "[[Transformatorji]]"
tags:
  - unfinished
aliases:
  - predavanje 5
---
# Struktura
Presečna krožna oblika je prikaza ne desni. Take oblike je zaradi tega, ker so ovitja okrogla, in ker tako dobimo zelo dobro faktor polnjenja železa. Tipične debeline lamel so: 0.35mm, 0.5mm. Z tako tanko lamelo dosežemo boljši izkoristek.

> [!image]
![[Trifazni transformator 2024-11-23 09.41.37.excalidraw]]
![[Trifazni transformator 2024-11-23 11.21.12.excalidraw]]

Transformatorje se tipično postavi v kotle, ki vključujejo varovalke, hladilno olje in priključna sponke. Manjše priključne sponke so za nizkonapetostno stran, večje so za visoko napetostno stran. Te imajo "kljobučki", da se prepreči preboj zaradi dežja ali snega. 

Za hlajenje se ponavadi uporablja olje, ki hladi, deluje pa tudi kot izolator. Zato je potrebna ekspanzijska posoda, da ima olje prostor za širjenje is krčenje. Ekspanzijska posoda, nam tudi omogoča plinsko analizo, s katero lahko analiziramo stanje navitja
# Vezava
Transformatorji so lahko vezani na več različnih načinov. Način kako so povezani konci navitji, nam pove kako deluje transformator, kolikšna bo fazna napetost, medfazna napetost in fazani kot med primarno is sekundarno stranjo.

Vezavo ki je na primarni strani označujemo z veliko črko, na sekundarni strani pa z malo.
## Zvezda (Y)
Ena stran navitji ne povezana na sponke transformatorja, druga je povezana skupaj. Tako dobimo kazalčni diagram, kjer je medfazna napetost enaka $U_{mf} = \sqrt{ 3 } U_{f}$. Ima tudi skupno zvezdišče, če želimo da nam je dostopna fazna napetost, potrebujemo napeljati zvezdišče ven iz transformatorja.
![[Trifazni transformator 2024-11-23 12.40.58.excalidraw]]

## Trikot (D)
Pri vezavi trikot imamo na voljo samo medfazno napetost. $U_{mf} = U_{f}$. Slabost te vezave je, da ne moremo priključiti enofaznih porabnikov, saj nimamo na voljo ničlišča.

**Kaj se zgodi, če priključiš enofazni porabnik med 2 sponki?**

![[Trifazni transformator 2024-11-23 13.04.34.excalidraw]]
## Cikcak (Z)
Tuljavo razpolovimo na vežemo konce polovic na poseben način. Za isto izhosnjo napetost potrebujemo 15 procetov vec navojev.
$$
U_{1W} = 2\frac{E_{1}}{2}\cos(30°) =2\frac{E_{1}}{2}\frac{\sqrt{ 3 }}{2} = 0.866 E_{1}
$$
$$
E_{1} = \frac{1}{0.866}U_{1W} = 1.153 U_{1W}
$$
![[Trifazni transformator 2024-11-23 13.24.07.excalidraw]]