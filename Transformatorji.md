---
creation date: 2025-02-25 09:34
last edit: 2025-03-08 13:32
id: 1740472482
aliases:
  - predavanje 2
ucb str: 49-52
related:
  - "[[Lenzovo pravilo]]"
  - "[[Gavsov zakon]]"
tags:
  - unfinished
---
Na [[Magnetni krog|prejšnjih predavanjih]] smo se naučili o magnetnem krogu, in o dušilki. Sedaj bomo dodali še eno navitje okoli stebra i z tem formirali transformator.
# Zgradba
Transformatorji so pogosto sestavljeni iz stebra in jermena. Tipično to dosežemo z EI konstrukcijo, kjer vzamemo list železa iz katerega izrežemo dva I-ja tako da ostaneta dva E-ja.  Imamo lahko konstrukcijo, kjer sta obes strani, visoko napetostna, in nizko napetostna na istem stebru. Tipično je visoko napetostna na zunanji strani zato da težje pride do preboja.

![[Transformatorji 2024-11-05 16.40.22.excalidraw.svg|70%]]
%%[[Transformatorji 2024-11-05 16.40.22.excalidraw.md|🖋 Edit in Excalidraw]]%%

# Obremenitev in ravnotežje transformatorja
Sedaj smo na sekundarno stran priključili breme. To breme še nima vpliva, ker je stikalo izklopljeno in ni sklenjen tokokrog. Ob tem času imamo na primarni strani napetost $u$, magnetilni tok $i_{m}$, v jedru glavni magnetni fluks $\Phi_{gl}$. Na sekundarni strani je pa samo inducirana napetost $e_{i2}$, ker imamo $N$ ovojev. Ko pa priključimo stikalo steče po sekundarni strani tok $i_{2}$, ki teče po navitju in skozi breme. 

![[1741433627.excalidraw.svg|70%]]
%%[[1741433627.excalidraw.md|🖋 Edit in Excalidraw]]%%

Tako kot na primarni strani, kjer imamo tok, ki teče po navitju, imamo sedaj na sekundarni strani tok ki teče po sekundarnem navitju. Posledica tega je magnetno polje. To magnetno polje nasprotuje glavnemu magnetnemu polju znotraj jedra transformatoja.

Sedaj bi lahko sklepali, da se je magnetno polje znotraj jedra spremenilo, saj magnetnemu polju, ki ga generira primarna stran nasprotuje magnetno polje sekundarne strani. 
$$
\Phi_{gl} = \Phi_{1} - \Phi_{2}
$$
Če bi predpostavili da je to res, potem bi bil fluks ki ga "čuti" primarna tuljava manjši in posledično, bi se na rpimarnem navitju inducirala manjša napetost $e_{i1}$. Ta inducirana napetost bi bila manjša od inducirane napetosti preden smo priklopili breme na sekundarni strani. Vemo pa, da je inducirana napetost na primarni strani enaka napetosti vira. Če ta dva dejstava sustavimo skupaj, bi pomenilo, da bi bila napetost vira višja od inducirane napetosti, to pa ne more veljati zaradi [[Kirchhoffova zakona]].
$$
u - e_{i_{1}} \ne 0
$$

Ko priključimo breme steče tok na sekundarni strani, kar pomeni da dovajamo neko energijo, kar pomeni, da moramo na primarni strani to energijo od nekod dobiti, in posledično se mora nekaj spremeniti. Dajmo pomisliti še enkrat. Sedaj vemo, da se znotraj jedra glavni fluks ne spremeni $\Phi_{gl}$, vendar imamo pa nasprotujoči fluks $\Phi_{2}$, katerega moramo kompenzirati. Ker je primarno navitje edini drugi vir magnetnega pretoka, lahko sklepamo, da se mora $\Phi_{1}$ povečati za $\Phi_{2}$. 
$$
\Phi_{1} = B A = \frac{HA}{\mu_{0}\mu_{r}} = \frac{N i_{1}A}{l_{sr} \mu_{0}\mu_{r}} 
$$
Ker nemore spreminjati same strukture transformatorja odpate nam ostane samo opcija spreminjanje primarnega tokova $i_{1}$. Čim priključimo breme na sekundarno stran se naš magnetilni tok $i_{m}$ spremeni v primarni tok $i_{1}$.

$$
\underline{I_{2}} = \frac{U_{2}}{\underline{Z_{b}}}
$$
Napetost ni podčrtana, ker je vodilni kazalec.

To velja v primeru, ko imamo napetostni vir, ki je tudi dovolj močen, da se napetost $u$ ne sesede ob preveliki obremenitvi.

Ko profesor pravi, da sekundarni tok ne vpliva na magnetni pretok znotraj jedra, se moti. Sekundarni tok vpliva na fluks znotraj jedra, vendar nas napetostni vir kompenzira za ta vpliv zato se fluks glavni ne spremeni. Glavni fluks znotraj jedra je kot neka toga palica, če jo na eno strni potisnemo, se bo tudi na drugi strani premaknila, kljub taku da se palica sama po sebi ni nič spremenila.

# Ravnotežje magnetnega vzbujanja
$$
\Theta_{1} = \Theta_{2} \Rightarrow I_{1}N_{1} = I_{2}N_{2} \Rightarrow \frac{I_{1}}{I_{2}} = \frac{N_{2}}{N_{1}}
$$
$$
I_{1} = I_{m} + I_{\delta} \Rightarrow I_{\delta} = I_{1} - I_{m}
$$
$$
I_{1} = \frac{N_{2}}{N_{1}}\frac{U_{2}}{Z_{b}}
$$
$I_{m}$ je odvisen od konstrukcije transformatorja.

# Nadomestno vezje %%Predavanje 3%% 
Nadomestno vezje je shema, ki nam pove, kje se nahajajo izgube v transformatorju.
![[Transformatorji 2024-11-05 16.56.07.excalidraw.svg]]
%%[[Transformatorji 2024-11-05 16.56.07.excalidraw.md|🖋 Edit in Excalidraw]]%%

$I_{1} - I_{2}' \Rightarrow  I_{10} = I_{od} + I_{m}$je tok prostega teka, ki magneti jedro in prinaša moč za izgube v železu.
$E_{1} = I_{m} 2 \pi f \frac{L}{G_{L}} = I_{m}X_{Gl}$
$I_{0d}$ je delovno komponenta toka prostega teka. $I_{0d}= \frac{P_{fe}}{E_{1}} =\frac{E_{1}}{R_{fe}}$. Kjer je $R_{fe} =\frac{E_{1}^{2}}{P_{fe}}$.
$P_{fe}$ predstavlja skupek vseh izgub znotraj železnega jedra.
$I_{m}$ je kompleksna komponenta toka prostega teka.

$X_{gl}$ je $\frac{E_{1}}{I_{m}}$, kar predstavlja glavno induktivno upornosti transformatorja.

Ker železno jedro hrani magnetno polje, moramo to predstaviti z elementom, ki hrani energijo, zato izberemo tuljavo.
## Redukcija %%Predavanje 3%%
Ker transformator spreminja nivo napetosti, bi na nadomestnem vezju odpovedali [[Kirchhoffova zakona|Kirchhoffovi zakoni]], zato izvedemo redukcijo. To storimo za inducirani napetosti, ki se nahajata na sredini nadomestnega vezja, v tem primeru redukcija na primarno stran, tako kot je na zgornji shemi vezja:

$$
E_{1} = E'_{2}
$$
Kjer je $E_{1}$ inducirana napetost na primarni strani transformatorja, $E'_{0}$ je pa reducirana inducirana napetost sekundarne strani. Pravo vrednost inducirane napetosti sekundarnega navitja se izračuna tako:
$$
E'_{2} = E_{2} \frac{N_{1}}{N_{2}}
$$
Zgornji dve enačbi vzamemo kot osnovo na nadaljnjo redukcijo drugih elementov v vezju.

$$
\begin{align}
I'_{2} = I_{2}\left(\frac{N_{2}}{N_{1}}\right)\\
R'_{2} = R_{2}\frac{{I_{2}}^{2}}{{I'_{2}}^{2}} = R_{2}\left( \frac{N_{1}}{N_{2}} \right)^{2}\\
X'_{L2} = X_{L2}\left( \frac{N_{1}}{N_{2}} \right)^{2}\\
X'_{C2} = X_{C2}\left( \frac{N_{1}}{N_{2}} \right)^{2}\\
Z_{b}' = Z_{b}\left(\frac{N_{1}}{N_{2}}\right)^{2}
\end{align}
$$
Pomembna lastnost redukcije je to, da se moč ohrani. Moč primarne strani je enaka pred i po redukciji, enako velja tudi za sekundarno stran. Tako se ohranijo moči, kar pomeni, da se ohranijo tudi izgubne moči. To je vidno v enačbi za redukcijo uporov.

**Pozor**, zgornji primeri so za redukcijo na primarno stran. To pomeni, da so vse napetosti in elementi v nadomestnem vezju prilagojene tako, da ustrezajo $E_{1}$. Da se tudi reducirati na sekundarno stran, kjer je osnova za redukcijo $E_{2}$. To storimo tako da, obrnemo ulomek v katerem ne nahaja število ovojev $N_{1}$ in $N_{2}$.

# Histerezne izgube %%Predavanje 4%%
Za to razlago bomo predpostavili, da so sponke sekundarnega navitja odprte, posledično na sekundarni $I_{2}$ ne teče (prosti tek). Naslednja poenostavitev bo, da je inducirana napetost enaka napetosti generatorja/pritisnjena napetost.
$$
U_{1} = E_{i} = 4.44 f N_{1} B\cdot A
$$

![[Transformatorji 2024-11-05 17.51.13.excalidraw]]
Slika je zelo gosta, vendar nam pove veliko o magnetnem polju znotraj jedra. Levo zgoraj je sinusni potek napetosti generatorja $U$. Ta napetost se prevede v magnetno polje $B$ s pomočjo [[Magnetni krog#Magična formula|magične formule]]. Desno zgoraj je vidna [[BH krivulja]], ki prikazuje relacijo med magnetnim poljem $B$ in jakost magnetnega polja $H$. Desno spodaj je narisan potek jakosti magnetnega polja skozi čas.

Z slike se da razbrati popačenje magnetnega polja, ki nastane zaradi nelinearnosti BH krivulje. S črno je narisana visoka napetosti, ki pripelje do visoke magnetnega polja $B$ in posledično preide v nasičenje krivulje. Preide iz linearnega dela, čez koleno, kjer je krivulja veliko bolj položna. Z zeleno je označena nizka napetost, ki pa obdrži svojo sinusno obliko, kar nikoli ne preide izven linearnega območja. 

![[Transformatorji 2024-11-05 18.07.54.excalidraw]]
Krivulja, ki se začne v izhodišču koordinatnega sistema, in potuje v točko 2, se imenuje deviška krivulja. Tako izgleda, ko prvič magnetimo železno jedro. Čez čas se krivulja spremeni, ker si magnetne domene "zapomnijo" kako so bile namagnetene. Posledica tega je, da imamo prisotno magnetno polje, tudi takrat, ko ga mi ne ustvarjamo samo. Ko je tok skozi tuljavo enak nič, je v jedru še vedno prisotno remanentno polje $B_{R}$. Velikost površine je odvisna od amplitude magnetenja.
$$
P_{h} = K_{h}\frac{f}{50}\left( \frac{B}{1.5T} \right)^{\alpha_{h}}m_{fe}
$$
Kjer je $K_{h}$ specifična histerezna izguba v $\left[ \frac{W}{kg} \right]$ železa pri frekvenci $50Hz$ in magnetnem polju $1.5T$, $m_{fe}$ je masa železnega jedra.

Če vzamemo osenčeno površino, in jo pomnožimo z frekvenco magnetenja $f$, dobimo energijo na sekundo $\left[ \frac{J}{s} = W \right]$, ki je moč histereznih izgub, ki se spreminja v toploto.

# Vrtinčne izgube %%Predavanje 4%%
Za lažje razumevanje si oglej [[Lenzovo pravilo]].

Ko imamo sklenjeno zanko, v kateri se spreminja magnetni fluks $\Phi$, se v zanki inducira napetost, ki povzroči tok. Ta tok bo deloval tako, da bo skušal nasprotovati spremembi magnetnega polja, ki prehaja skozi zanko. Zanka se tako "upira" spremembi fluksa.
$$
\frac{d\Phi(t)}{dt} = e_{i}
$$

Tok bo največji, ko bo sprememba fluksa največja. Če se fluks spreminja sinusno, bo tok enak nič, ko bo fluks dosegel svojo maksimalno vrednost.

![[Transformatorji 2024-11-12 16.54.55.excalidraw]]

Zaradi sprememb fluksa se v železnem jedru inducirajo vrtinčni tokovi.

![[Transformatorji 2024-11-12 17.12.44.excalidraw]]

Da bi zmanjšali te vrtinčne tokove, prilagodimo konstrukcijo transformatorja. Namesto enega velikega železnega jedra uporabimo slojevito zgrajen transformator. Pločevine, ki imajo neprevodni zunanji sloj, zlagamo skupaj, kar ustvarja železno jedro z lamelami. Te lamele zmanjšajo nastanek vrtinčnih tokov, ker zmanjšajo velikost zank v jedru. Z drugimi besedami, zmanjšamo Ko so plasti jedra ločene, se poveča upornost za ustvarjanje in širjenje vrtinčnih tokov. Vsaka plast jedra deluje kot nekakšen "prekinjevalec" za vrtinčne tokove, ki so prisotni v jedru.

$$
RI=R\uparrow I\downarrow
$$
![[Transformatorji 2024-11-12 17.20.46.excalidraw]]

Vrtinčni tok $i_{vr}$ je sorazmeren z inducirano napetostjo $e_{i}$, ta pa je sorazmerna z magnetnim poljem $B$ in frekvenco $f$ tako kot pravi magič formula.

Vrtinčne izgube $P_{vrt}$ so sorazmerne z kvadratom vrtinčnih tokov $I_{vr}^{2}$. Posledično lahko trdimo, da se izgube spreminjajo sorazmerno s kvadratom magnetnega polja $B^{2}$ in frekvence $f^{2}$.

$$
P_{ver} = K_{vr}\left( \frac{f}{50Hz} \right)^{2}\left( \frac{B}{1.5T} \right)^{2}m_{fe}
$$
kjer je $K_{vr}$ faktor materiala. Ta je odvisen od materiala jedra transformatorja. Enota je $\left[ \frac{W}{kg} \right]$. Tipične debeline lamel so med $0.2$ in $0.6$ mm. Frekvenco $f$ in magnetno polje $B$ normiramo na standardne vrednosti $50Hz$ in $1.5T$ za običajno računanje izgub.
# Izgube v navitju
**TODO**
To je treba znati za kratek stik.
# Skupne izgube
$K_{fe}$ je lastnost železa in je skupek $K_{vr}$ in $K_{h}$.

$$
P_{fe}=P_{h} + P_{vrt} = K_{fe}\frac{f}{50}\left( \frac{B}{1.5} \right)^{\alpha_{n}}m_{fe}
$$
# Izkoristek
$$
\eta = \frac{Poddana}{Psprejeta} < 1
$$