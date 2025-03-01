---
creation date: 2025-02-19 13:37
last edit: 2025-03-01 16:20
id: 1739968659
aliases:
  - predavanje 1
ucb str: 12-28
related: 
tags:
  - unfinished
---
# Enosmerni magnetni krog
Preprosto magnetno jedro z zračno režo je na spodnji sliki. 
![[Magnetni krog 2024-11-02 09.34.50.excalidraw.svg|70%]]
%%[[Magnetni krog 2024-11-02 09.34.50.excalidraw.md|🖋 Edit in Excalidraw]]%%

Okoli železnega jedra imamo navitje, ki ima $N$ ovojev in deluje kot tuljava. Ta generira magnetno polje. To navitje je napajano s strani enosmernega generatorja, ki vzbudi magnetilni tok $I_{m}$ in napetost $U$ po navitju. Ker je vir enosmeren se lahko izračuna tok preko [[Ohmov zakon|ohmovega zakona]] $I_{m}=\frac{U}{R_{nav}}$, kjer je $R_{nav}$ upornost navitja.

# Povezava z električnimi vezji
Z pomočjo [[Amperov zakon|amerovega zakona]] lahko izračunamo stanje v magnetnih krogih. Ker je enčaba, ki jo podaja amperov zakon zapletena bomo predpostavili določene poenastavitve:
- Magnetno polje $\vec{B}$ je v feromagnetnem jedru in v zračni reži **homogeno**,
- **linearna karakteristika** (pred kolenom ali pred nasičenjem) $BH$ [[BH krivulja|krivulje]], $B=\mu_{0} \mu_{r} \cdot H \Rightarrow y = k \cdot x; k = \mu_{0}\mu_{r}$
- magnetno polje je **vzporedno** normali površine prereza: $\vec{B} \parallel d\vec{A}$ ali $\vec{H}\parallel \vec{l}$.

Tako se celotna enčba poenostavi na:
$$
H \cdot l_{sr} = N \cdot I_{m}
$$

kjer je $l_{sr}$ srednja zanka skozi železno jedro, ki jo lahko sestavimo iz $l_{fe}$ in $l_{zr}$. Tako dobimo poenostavljeno enačbo za naš zgornji primer:
$$
H_{fe} \cdot l_{fe} + H_{zr} \cdot l_{zr} = N \cdot I_{v}
$$

kjer pomeni oznaka $fe$ veličine vezane na železo, in $zr$ veličine v zraku. $N$ je število ovojev, ki seka površino, ki jo lahko napnemo na zanko $l_{sr}$. Z drugimi besedami, število ovojev okoli železnega jedra.

$N \cdot I_{v}$ lahko interpretiramo kot magnetno vzbujanje ali magnetno napetost, medtem ko $\sum H_{i}l_{i}$ kot padce napetosti. Tako smo formulirali magnetno vezje, ki ga lahko razumemo z pomočjo [[Ohmov zakon|ohmovih]] in [[Kirchhoffova zakona|kirchhoffovih zakonov]].

$$
U = R \cdot I \Rightarrow \Theta = \Phi \cdot R_{m}
$$
$$
\Phi R_{mfe} + \Phi R_{mzr} = \Theta_{mv} = I_{v} \cdot N
$$
kjer je $R_{m}$ magnetna upornost ali **reluktanca**. Tako lahko narišemo zgornjo dušilko v obliki električnega vezja. Vezje zgornjega primera bi tako izgledalo:

![[Magnetni krog 2024-11-02 12.30.49.excalidraw.svg| 70%]]
%%[[Magnetni krog 2024-11-02 12.30.49.excalidraw.md|🖋 Edit in Excalidraw]]%%

$\mu_{fe}$ nam pove relativno permiabilnost železa. Mi smo predpostavili, da je linearen ($\mu_{fe}$ je konstanten), vendar v resnici ni. Za več si oglej [[BH krivulja]]. Ker je $\mu_{fe}$ v rangu nekaj tisoč lahko rečemo, da je magnetna upornost železa zanemarljivo v primerjavi z upornostjo zračne reže.
$$
\frac{R_{mfe}}{R_{mzr}} = \frac{\frac{1}{\mu_{0}\mu_{fe}}}{\frac{1}{\mu_{0}}} = \frac{1}{\mu_{fe}} \approx 0
$$
Tako lahko izračunamo flux $\Phi$, kjer prevladuje zračna reža:
$$
\Phi =\frac{I\cdot N}{R_{mfe}+R_{mzr}} = \frac{I\cdot N}{R_{mzr}} =  \frac{U_{el}}{R_{el}}N \frac{\mu_{0}A_{zr}}{l_{zr}}
$$
# Magnetno polje v zračni reži
**Bomo zanemarili**, saj predpostavimo, da nimamo zračnih rež. To je bolj kot zanmivost.

Pri prehodu magnetnega polja iz železnega jedra v zračno režo in nazaj se pojavi sprememba efektivne površine, skozi katero teče magnetno polje. Ker magnetno polje išče najkrajšo pot med dvema kosoma železa, se bo rahlo "napihnilo", kar pomeni, da se površina, skozi katero teče, poveča. Ker je flux $\Phi$ v jedru in v zračni reži enaka, površina $A$ pa se spremeni, se posledično spremeni tudi gostota magnetnega pretoka $B = \frac{\Phi}{A}$. Zaradi povečanja površine v zračni reži se lahko reluktanca zmanjša, kar vpliva na celotno magnetno vezje.

![[Magnetni krog 2024-11-02 13.05.34.excalidraw]]

# Stresano magnetno polje
Ko navitje generira magnetno polje, bo ta iskal najkrašo pot, da se zaključi njegova zanka. Zaradi tega, bo del magnetnega polja pobegnil našemu železnemu jedru. Za nas to predstavlja izgube, ker želimo celotni magnetni pretok skozi jedro.
![[Magnetni krog 2024-11-02 13.47.52.excalidraw.svg|70%]]
%%[[Magnetni krog 2024-11-02 13.47.52.excalidraw.md|🖋 Edit in Excalidraw]]%%

# Izmenični magnetni krog
Sedaj pa dajmo zamenjati enosmerni napetostni vir $U$ za izmeničnnega $u(t) = \hat{U}\sin(t)$.
![[1740830887.excalidraw.svg|70%]]
%%[[1740830887.excalidraw.md|🖋 Edit in Excalidraw]]%%
Ko priključimo napetostni vir steče tok po bakrenih žicah, ker imajo neko upornost. Posledica toka je kreacija magnetnega polja znotraj navitja in železnega jedra. Ker imamo sklenjeno zanko in spreminjajoče magnetno polje se na tej zanki inducija napetost. Ta inducirana napetost mora biti po [[Kirchhoffova zakona|kirchoffu]] enaka napetosti, ki jo podaja vir. Torej lahko rečemo, da mora biti tok $I_{m}$ take vrednosti, da bo inducirana napetost enaka napetosti vira.

$I_{m} = $

Ker imamo izmenični vir napetosti $u$ imamo tudi izmenični tok $i_{m}$, ki teče po navitju, posledično je gostota magnetnega polja $B$ znotraj jedra tudi izmenična. Prva polovica periode kaže magnetno polje v eno smer, drugo polovico pa kaze v nasprotno.

![[1740836360.excalidraw.svg|70%]]
%%[[1740836360.excalidraw.md|🖋 Edit in Excalidraw]]%%
Posledica izmeničnega magnetnega polja in zaprte zanke je inducirana napetost. O tem govori [[faradej zakon]]: 
$$
e_{i} = -\frac{d \psi}{dt} = -\frac{d (N \Phi)}{dt} \approx -N\frac{d\Phi}{dt}
$$

$N$ lahko premaknemo izven odvoda takrat, ko zanemarimo stresano magnetno polje. [[Magnetni krog#Stresano magnetno polje|Stresano magnetno]] polje se razlikuje od [[Magnetni krog#Magnetno polje v zračni reži|magnetnega polja v zračni reži]]. Sresano magnetno polje povzroče izgube, saj ne gre celotno magnetno polje skozi jedro, medtem ko polje v zračni reži samo spremeni fluks $\Phi$.

Prej smo izrazili magnetni fluks kot:
$$\Phi = \frac{I_{m}N}{R_{mfe} + R_{zr}}$$
Sedaj imamo pa izmenični tok, ki ga zapišemo kot $i_{m} = \hat{I}_{m}\cdot \sin(\omega t)$, kjer je $\hat{I}_{m}$ amplituda toka. Tako lahko sestavimo enačbo
$$\Phi(t) = \frac{\hat{I}_{m}N}{R_{mfe} + R_{zr}} \cdot \sin(\omega t)$$

Kadar obravnavamo izmenično magnetno polje, se pojavi inducirana napetost, ki se izračuna kot[^1]:
$$
e_{i} = \frac{d \Psi}{dt}= \frac{d\Phi N}{dt} \underbrace{=}_{*1} N\frac{d\left( \int_{A}\vec{B} d\vec{A}\right)}{dt} \underbrace{\approx}_{*2} N\frac{d(B\cdot A)}{dt} \underbrace{=}_{*3} NA \frac{dB}{dt}
$$
1. Zanemarimo stresano magnetno polje,
2. $B$ homogen in $\vec{B} \parallel d\vec{A}$,
3. Presek je konstanten
$$
B(t) = \frac{\Phi(t)}{A} = \underbrace{\frac{\hat{I}_{m}N}{(R_{mfe} + R_{mzr})A}}_{\hat{B}}\sin (\omega t)
$$
$$
e_{i}(t) = N A \frac{d(\hat{B}\sin(\omega t))}{dt} = \underbrace{NA\hat{B}\;\omega}_{amplituda\;(\hat{e_{i}})}\cos(\omega t)
$$

**Od sedaj naprej bodo magnetne količine vedno podane kot amplitudna vrednost, električne pa kot efektivne vrednosti.** Ker, za računanje električne moči uporabljamo enačbo $P = U \cdot I$, kjer lahko zamenjamo $U$ in $I$ za effektivne vrednosti, če nimamo enosmernih pogojev. Za magnetne veličine pa uporabljamo amplitudo, zaradi [[BH krivulja|BH krivulje]], saj ni linearna, in nam bi effektivna vrednost prikazala napačno sliko v nasičenju.

Ko računamo [[Efektivne vrednosti|efektivno vrednosti]] sinusnega signala dobimo $\overline{X} = \frac{\hat{X}}{\sqrt{ 2 }}$.
# Magična formula
Zgornjo enačbo lahko dopolnimo z $\omega = 2 \pi f$ in relacijo, da je efektivna vrednost enaka $\frac{1}{\sqrt{ 2 }}$. Tako dobimo:
$$
E_{i} = \frac{2 \pi}{\sqrt{ 2 }} f N A B = 4.44\; N f \hat{}B A
$$
Ta enačba velja za ko vpoštevamo 3 prej omenjene poenostavitve, linearne razmere in homogeno polje, ter sinusno spreminjajoče veličine.

Magična formula nam pove, da na magnetni pretok vplivamo samo z effektivno vrednostjo napetosti $u$, frekvenco $f$, število ovojev $N$ in presekom jedra $A$. Če spreminjamo zračno režo $\delta$, ne spreminjamo magnetnega pretoka $\Phi$. 

Zračna reža pa vpliva na magnetilni tok $I_{m}$, to je vidno iz enačbe:
$$
\hat{\Phi} = \frac{\Theta}{R_{mzr}} = \frac{\sqrt{ 2 }I_{m}N}{R_{mzr}}
$$
Sedaj bi se lahko vprašali, kako to, da zračna reža ne vpliva na fluks, če je v enačbi jasno vidno, da je odvisna od reluktance zračne reže. Pomembno dejstvo, ki ga profesor ni povedal, je to, da to velja za napetostni vir. Če bi imeli tokovni vir, bi bila obravnava drugačna.

Če nadaljujemo:
$$
I_{m} = \frac{\hat{\Phi}R_{mzr}}{\sqrt{ 2 }N} =\frac{E_{i}}{\underbrace{2 \pi f}_{\omega}}\frac{R_{mzr}}{N^{2}} = \frac{E_{i}}{\omega L} = \frac{E_{i}}{X_{L}}
$$
Po definiciji je $L = \frac{\Phi}{I}$.


---
Naslednje poglavje: [[Transformatorji]]

[^1]: [Elektromagnetna indukcija - Wikipedija, prosta enciklopedija](https://sl.wikipedia.org/wiki/Elektromagnetna_indukcija)