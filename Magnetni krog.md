---
creation date: 2025-02-19 13:37
last edit: 2025-02-21 13:33
id: 1739968659
aliases:
  - predavanje 1
ucb str: 12-28
related: 
tags:
  - unfinished
---
# Enosmerni magnetni krog 
![[1740141209.excalidraw.svg]]
%%[[1740141209.excalidraw.md|🖋 Edit in Excalidraw]]%%
![[1740140972.excalidraw.svg]]
%%[[1740140972.excalidraw.md|🖋 Edit in Excalidraw]]%%
![[Magnetni krog 2024-11-02 09.34.50.excalidraw]]

Okoli železnega jedra imamo navitje, ki deluje kot tuljava, ki generira magnetno polje in fluks (magnetno polje krat površina za homogene razmere). To navitje je napajano s strani enosmernega generatorja, ki vzbudi tok $I_{v}$ in napetost $U$ po navitju. Ker je vir enosmeren se lahko izračuna tok preko [[Ohmov zakon|ohmovega zakona]] $I_{v}=\frac{U}{R_{nav}}$, kjer je $R_{nav}$ upornost navitja.

# Povezava z električnimi vezji
Z pomočjo [[Amerov zakon|amerovega zakona]] bomo računali stanje v magnetnih krogih. Ker je enčaba, ki jo podaja amperov zakon zapletena bomo predpostavili določene poenastavitve:
- Homogeno magnetno polje $\vec{B}$ v feromagnetnem jedru in v zraćni reži,
- linearna karakteristika (pred kolenom ali pred nasičenjem) $BH$ [[BH krivulja|krivulje]], $B=\mu_{0} \mu_{r} \cdot H \Rightarrow y = k \cdot x; k = \mu_{0}\mu_{r}$
- magnetno polje je vzporedno normali površine prereza: $\vec{B} \parallel d\vec{A}$ ali $\vec{H}\parallel \vec{l}$.

Tako se l evi del enačbe poenostavi:
$$
\oint_{\mathcal{L}}\vec{H}d \vec{l} = H \cdot l_{sr}
$$
$$
\oint_{\mathcal{L}}\vec{H}d \vec{l}  = \int_{A} \vec{J}d\vec{A}
$$
%% TODO: Vrednosti intergrala na desni strani enačbe pa je tok ki prebada površino A. V nasem primeru je to I * N %%

kjer je $l_{sr}$ srednja zanka skozi železno jedro, ki jo lahko sestavimo iz $l_{fe}$ in $l_{zr}$. Tako dobimo poenostavljeno enačbo za naš zgornji primer:
$$
H_{fe} \cdot l_{fe} + H_{zr} \cdot l_{zr} = N \cdot I_{v}
$$
kjer pomeni oznaka $fe$ veličine vezane na železo, in $zr$ veličine v zraku. $N$ je število ovojev ki seka površino, ki jo lahko napnemo na zanko $l_{sr}$. Z drugimi besedami, število ovojev okoli železnega jedra.

$N \cdot I_{v}$ lahko interpretiramo kot magnetno vzbujanje ali magnetno napetost, medtem ko $\sum H_{i}l_{i}$ kot padce napetosti. Tako smo formulirali magnetno vezje, ki ga lahko razumemo z pomočjo [[Ohmov zakon|ohmovih]] in [[Kirchhoffova zakona|kirchhoffovih zakonov]].

$$
U = I \cdot R \Rightarrow \Theta = \Phi \cdot R_{m}
$$
$$
\Phi R_{mfe} + \Phi R_{mzr} = \Theta_{mv} = I_{v} \cdot N
$$
kjer je $R$ magnetna upornost ali reluktanca.

Vezje zgornjega primera bi tako izgledalo:

![[Magnetni krog 2024-11-02 12.30.49.excalidraw]]

$\mu_{fe}$ nam pove relacijo med magnetnim polje ${B}$ in gostoto magnetnega pretoka $H$. Mi smo predpostavili, da je ta relacija linearna ($\mu_{fe}$ je konstanten), vendar v resnici ni. Za več si oglej [[BH krivulja]].
Ker je $\mu_{fe}$ v rangu nekaj tisoč lahko rečemo, da je magnetna upornost železa zanemarljivo v primerjavi z upornostjo zračne reže.
$$
\frac{\frac{1}{\mu_{0}\mu_{fe}}}{\frac{1}{\mu_{0}}} = \frac{R_{mfe}}{R_{mzr}} \Rightarrow \frac{1}{\mu_{fe}}= \frac{R_{mfe}}{R_{mzr}}
$$
Tako lahko izračunamo magnetni pretok, kjer prevladuje zračna reža:
$$
\boxed{
\Phi =\frac{I\cdot N}{R_{mfe}+R_{mzr}} = \frac{I\cdot N}{R_{mzr}} =  \frac{U_{el}}{R_{el}}N \frac{\mu_{0}A_{zr}}{l_{zr}}
}
$$
**Pozor** $U$ in $R$ sta električni veličini.

# Magnetno polje v zračni reži
Iz zgornjih enačb lahko zapišemo:
$$
\Phi_{zr} = \Phi_{fe} \Rightarrow B_{zr}A_{zr} = B_{fe}A_{fe}
$$
vendar ker magnetna polja $B$ nista enaka, pomeni da tudi površini železa in zraka nista enaki. Ker je $B_{zr}$ manjši, mora biti $A_{zr}$ večji, da dobimo enakost.
![[Magnetni krog 2024-11-02 13.05.34.excalidraw]]
%% TODO: Make image smaller %%

# Izmenični magnetni krog
Ker imamo izmenični vir napetosti imamo tudi izmenični tok, ki teče po navitju, posledično je magnetno polje znotraj jedra tudi izmenično. Prva polovica periode kaže magnetno polje v eno smer, drugo polovico pa kaze v nasprotno.
$$
\frac{d \psi}{dt} = \frac{d (N \Phi)}{dt} \approx N\frac{d\Phi}{dt}
$$
$N$ lahko premaknemo izven odvoda takrat, ko zanemarimo stresano magnetno polje. Stresano magnetno polje se razlikuje od [[Magnetni krog#Magnetno polje v zračni reži|magnetnega polja v zračni reži]], saj stresano magnetno polje je tisto, ki ne teče znotraj železnega jedra, ki je obkrožen z navitjem.
![[Magnetni krog 2024-11-02 13.47.52.excalidraw]]
Prej smo izrazili magnetni fluks kot $\Phi = \frac{I_{m}N}{R_{mfe} + R_{zr}}$, sedaj imamo pa izmenični tok, ki ga zapišemo kot $i_{m} = \hat{I}_{m}\cdot \sin(\omega t)$, kjer je $\hat{I}_{m}$ amplituda toka. Tako lahko sestavimo enačbo $\Phi(t) = \frac{\hat{I}_{m}N}{R_{mfe} + R_{zr}} \cdot \sin(\omega t)$.

Kadar obravnavamo izmenično magnetno polje, se pojavi inducirana napetost, ki se izračuna kot[^1]:
$$
e_{i} = \frac{d \Psi}{dt}= \frac{d\Phi N}{dt} = N\frac{d\left( \int_{A}\vec{B} d\vec{A}\right)}{dt} \underbrace{\approx}_{{\vec{B} \parallel d\vec{A}}} N\frac{d(B\cdot A)}{dt} = NA \frac{dB}{dt}
$$
$$
B(t) = \frac{\Phi(t)}{A} = \underbrace{\frac{\hat{I}_{m}N}{(R_{mfe} + R_{mzr})A}}_{\hat{B}}\sin (\omega t)
$$
$$
e_{i}(t) = N A \frac{d(\hat{B}\sin(\omega t))}{dt} = \underbrace{NA\hat{B}\;\omega}_{amplituda\;(\hat{e_{i}})}\cos(\omega t)
$$
Kjer je $\psi = N \cdot \phi$ magnetni sklep in nam pove kolikokrat objamemo jedro z tuljavo. 
**Od sedaj naprej bodo magnetne količine vedno podane kot amplitudna vrednost, medtem ko električne pa kot efektivne vrednosti.** Ko računamo efektivno vrednosti sinusnega signala dobimo $\overline{X} = \frac{\hat{X}}{\sqrt{ 2 }}$.
# Magična formula
Zgornjo enačbo lahko dopolnimo s $\omega = 2 \pi f$ in z relacijo, da je efektivna vrednost enaka $\frac{1}{\sqrt{ 2 }}$. Tako dobimo:
$$
E_{i} = \frac{2 \pi}{\sqrt{ 2 }} f N A B = 4.44\; N f \hat{}B A
$$
Ta enačba velja za homogene razmere v jedru, vse 3 prej omenjene poenostavitve, linearne razmere, in sinusno spreminjajoče veličine.

Naša neznanka je $\Phi = BA$:
$$
\Phi = \frac{E_{i}}{4.44 N f}
$$
inducirana napetost je skoraj enaka vzbujani napetosti $E_{i} = U$:
$$
\Phi = \frac{U}{4.44 N f}
$$

![[Magnetni krog 2024-11-02 14.42.51.excalidraw]]
$$
B= \frac{E_{i}}{4.44 fNA}
$$
Če hočemo povečati magnetno polje znotraj železa moramo povečati napajanje $U$, lahko pa tudi zmanjšamo frekvenco.

---
Naslednje poglavje: [[Transformatorji]]

[^1]: [Elektromagnetna indukcija - Wikipedija, prosta enciklopedija](https://sl.wikipedia.org/wiki/Elektromagnetna_indukcija)