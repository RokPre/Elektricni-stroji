---
related:
  - "[[Transformatorji]]"
tags:
  - unfinished
aliases:
  - predavanje 3
  - Kazalčni diagram transformatorja
---
# Poenostavitev nadomestnega vezja
Imamo nadomestno vezje transformatorja, ki smo ga razložili v [[Transformatorji|predavanje 2]]. Predpostavimo, da imamo breme z zelo visoko impedanco $Z_{b} \to \infty$ $(R+X+L)$, praktično lahko rečemo, da imamo odprte sponke, ali da transformator obratuje v prostem teku. Če je magnetno jedro brez zračnih rež potem ima zelo majhne izgube, in lahko rečemo, da je magnetilni tok zelo majhen $I_{m} \to 0$. Ker je magnetilni tok tako majhen, ga lahko pomaknemo na začetek vezja.

![[Nadomestno vezje transformatorja 2024-11-16 09.21.33.excalidraw]]
Sedaj ko smo prestavili magnetilno vejo, lahko tudi združimo skupaj elemente, ki predstavljajo navitje $X_{\sigma_{1}}+X_{\sigma_{2}}' = X_{\sigma_{k}}$ ter $R_{1}+R_{2}'=R_{k}$.

![[Nadomestno vezje transformatorja 2024-11-16 09.29.36.excalidraw]]

Torej najprej smo predpostavili, da je magnetno jedro transformatorja kvalitetno zato, da smo ga lahko premaknili na začetek vezja, potem združimo elemente, ki predstavljajo navitje, na koncu pa zanemarimo magnetilno vejo, zaradi iste predpostavke kot prej, da je jedro kvalitetno. 

**Q: Zakaj nismo že na začetku zanemarili magnetilne veje?**
A: 

# Vloga elementov v vezju
## Odprte sponke
Ponovno imamo transformator v prostem teku (samo volt meter). Z pomočjo kazalčnega diagrama, lahko preprosto izračunamo $\varphi_{0}$, kar nam omogoča izračun [[delovne komponente moči]].
**Zakaj smo zanemarili navitje?**
![[Nadomestno vezje transformatorja 2024-11-16 09.49.15.excalidraw]]

## Kratek stik
Sedaj imamo kratek stik (samo amper meter). V tem primeru je tok na sekundarni strani zelo velik, kar pomeni, da se nam upira navitje. Ker je magnetni tok tako majhen, lahko zanemarimo centralno vejo nadomestnega vezja.

![[Nadomestno vezje transformatorja 2024-11-16 10.05.48.excalidraw]]

# Kazalčni diagram najbolj poenostavljenega vezja
![[Nadomestno vezje transformatorja 2024-11-16 10.27.26.excalidraw]]

# Kazalčni diagram nadomestnega vezja
Za lažje risanje kazalčnega diagrama si izberemo veličino, ki je najbolj oddaljena od napetostnega vira. Zato si izberemo $I_{2}'$ kot osnovo za vse ostale veličine. Začnemo na desni in se po korakih premikamo levo.

1. Za začetek si izberemo veličino, ki je najbolj oddaljena od napetostnega vira, to je tok na sekundarni strani $I_{2}'$. Tok $I_{2}'$ postavimo kot osnovo za vse ostale veličine. Ker gre za osnovno veličino, jo narišemo vodoravno,
2. napetost na bremeni $U_{2}'$ je fazno zamaknjena na tok $I_{2}'$ za kot $\varphi_{b}$, ki je odvisen od lastnosti bremena,
3. padec napetosti na upornosti $R_{2}'$ je v fazi z tokom $I_{2}'$, padec na reaktanci $X_{\sigma 2}'$ je pa pravokotno na tok $I_{2}'$. Te padce rišemo na koncu $U_{2}'$.
4. skupni seštevek vseh napetosti na desni strani vezja $U_{2}' + U_{R2}+U_{X_2}$ je enak reducirani inducirani napetosti na sekundarni strani $E_{2}'$,
5. $E_{2}'$ nam podaja osnovo za risanje veličini, ki tečejo skozi magnetno jedro. Narišemo magnetilni tok $I_{m}$ in $I_{od}$ pravokotno na $E_{2}'$ in vzporedno na $E_{2}'$, skupni seštevek teh tokov je $I_{10}$.
6. Na primarni strani je tok $I_{1}$ enak vsoti sekundarnega toka $I_{2}'$ in toka $I_{10}$, ki teče skozi sredinsko vejo.
7. Padec napetosti na primarnem navitju je sestavljen iz uporne komponenta $U_{R1}$ in reaktance $U_{X1}$, kjer je $U_{R1}$ v fazi s tokom $I_{1}$, $U_{X1}$ pa je pravokotna na $I_{1}$.
8. Na koncu še narišemo $U_{1}$, ki je enak vsoti napetosti $E_{1}+U_{R1} + U_{X1}$.
![[Nadomestno vezje transformatorja 2024-11-16 10.41.58.excalidraw]]

# Prosti tek
str. 62
# Kratek stik
str. 64
# Obremenjen trafo
## Induktivna obremenitev
## Kapacitivna obremenitev