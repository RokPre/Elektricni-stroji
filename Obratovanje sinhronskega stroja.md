---
related: 
tags:
  - unfinished
aliases:
  - predavanje 8
---
# Prosti tek sinhronskega stroja
Prosti tek sinhrnokesga stroja pomeni, da ni priključen na nobeno obremenitev. Če je v generatorskem režimu ima odprte sponke, ustvari napetost vendar ne teče tok, če je motornem režimu, nima nobene mehanske obremenitve na gredi, se gred vrti v prazno.

Tok rotorja povrzroči fluks rotorja, ta dva sta v fazi drug z drugim. Fluks kroži kar povzroči spreminjanje fluksa. Ta sprememba inducira napetost v statorskem navitju.

Histrost vrtenja električnega polja okoli statorja doloća hitrost vrtenja rotorja in število polovih parov:
$$
n_{meh} \cdot p = n_{mag}
$$
kjer sta $n$ hitrosti vrtenja in $p$ stevilo polovih parov.

![[1734772954.excalidraw.svg]]
%%[[1734772954.excalidraw.md|🖋 Edit in Excalidraw]]%%

# Sinhroniziranje sinhronskega stroja na omrežje
Za priklop sinhronskega generatorja na omrežje moramo zagotoviti, da je razlika med inducirano napetostjo na stroju in napetostjo omrežja čim manjša. Če razlika ni zadostno majhna, bi to povzročilo zelo velik tok znotraj generatorja, kar je podobno pojavu, ki se zgodi pri vključitvi transformatorja (t.i. [[Vklopni pojav transformatorja]]). Zato med omrežjem in generatorjem uporabljamo ničelni voltmeter, ki meri razliko med napetostma. Naš cilj je, da uskladimo jakost, frekvenco in fazo napetosti. Če niso usklajene, voltmeter ne bo kazal ničelne vrednosti, kar pomeni, da generator ni sinhroniziran z omrežjem.

S pomočjo magične formule lahko izračunamo, katere parametre moramo prilagoditi, da bo generator pripravljen za priklop na omrežje. Če amplitudi napetosti nista usklajeni, moramo spremeniti vzbujalni tok, ki teče skozi rotor generatorja. Če pa se frekvenci ne ujemata, moramo prilagoditi hitrost turbine. S tem se spremeni tudi amplituda inducirane napetosti, saj je napetost neposredno sorazmerna s frekvenco $E \propto f$. To pomeni, da moramo poleg hitrosti turbine prilagoditi tudi vzbujalni tok, da zagotovimo usklajenost z omrežjem.

![[1734773900.excalidraw.svg]]
%%[[1734773900.excalidraw.md|🖋 Edit in Excalidraw]]%%
![[1734776286.excalidraw.svg]]
%%[[1734776286.excalidraw.md|🖋 Edit in Excalidraw]]%%
# Nadomestno vezje
## Prosti tek
![[1734782133.excalidraw.svg]]
%%[[1734782133.excalidraw.md|🖋 Edit in Excalidraw]]%%
## Preuzbujanje
V tem primeru imamo visoko inducirano napetost, ki je višja od napetosti omrežja, to smo dosegli z visokim vzbujalnim toko $I_{v}$. Zaradi te razlike v napetosti $\Delta U$ stroj "oddaja" tok $I_{1}$. Ta tok je kapacitivnega značaja in je pravokoten na $\Delta U$. Stroj sedaj oddaja čisto jalovo moč induktivnega značaja. Omrežje stroj zaznava kot kondenzator. To jalovo moč potrebujejo porabniki induktivnega značaja.

![[1734783015.excalidraw.svg]]
%%[[1734783015.excalidraw.md|🖋 Edit in Excalidraw]]%%
## Poduzubujanje
Za razliko od prejšnjega stanja, ko smo stroj preuzbujali, ga zdaj poduzbujamo. Inducirana napetost $E_{f}$​ je nižja od napetosti omrežja $U$, zato je razlika napetosti $\Delta U$ obrnjena navzdol. Tok in razlika napetosti sta pravokotna, saj imata kapacitivni značaj: $E_f - U \perp I_1$. Omrežje sedaj stroj vidi kot tuljavo/dušilko (induktivno), saj tok "prehiteva" omrežno napetost. Energija, ki jo stroj oddaja, se uporablja za polnjenje kondenzatorjev.

**Kompenzator jalove energije** 
![[1734783921.excalidraw.svg]]
%%[[1734783921.excalidraw.md|🖋 Edit in Excalidraw]]%%
## Jalova obremenitev
## Delovna obremenitev
Če hočemo odddajati delovno moč v omrežje morata biti tok in omrežna napetost vzporedna $I \parallel U$. To dosežemo tako, da je faza inducirane napetosti in omrežne napetosti ne ujemata več. 
![[1734781779.excalidraw.svg]]
%%[[1734781779.excalidraw.md|🖋 Edit in Excalidraw]]%%

Če imamo razliko napetosti $\Delta U$, ki je vodoravna in kaže na desno, tok $I_{1}$ pa kaže navzdol, imamo stroj, ki troši energijo, in obratuje kot motor.