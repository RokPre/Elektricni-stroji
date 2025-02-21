---
related:
tags:
  - unfinished
aliases:
  - predavanje 7
---
# Uvod
Sinhronski stroji, za razliko od transformatorjev, ki pretvarjajo električno energijo v električno, pretvarjajo električno v mehansko in obratno.
# Povezava z [[Transformatorji]]

> [!image]
![[Drawing 2024-11-30 10.16.38.excalidraw]]
![[Sinhronski stroji 2024-11-30 10.22.40.excalidraw]]
$$\begin{array}{c c}
U_1 + E_1 = 0 && I_1^{\prime} > I_1 \\
E_1 = N_1 \frac{d\Phi}{dt} &&  \Phi^{\prime} = \Phi
\end{array}
$$


> [!image]
![[Sinhronski stroji 2024-11-30 10.32.22.excalidraw]]
![[Sinhronski stroji 2024-11-30 10.36.47.excalidraw]]
$$\begin{array}{c c}
E_2 = N_{2}\frac{d\Phi}{dt} && \Phi' < \Phi \\
 && E_{2}' < E_{2}
\end{array}
$$
# Struktura
Sinhronski stroj je sestavljen pa je iz dveh glavnih komponent: statorja in rotorja. Stator je zunanji del stroja in predstavlja nepremični del, medtem ko rotor, ki se nahaja v notranjosti, predstavlja premikajoči se del.

V statorju ni navitja za vzbujanje, saj sinhronski stroji običajno delujejo kot generatorji, kjer prevajajo mehansko energijo v električno. Z vrtenjem rotorja preko mehanskega pogona se ustvarja spremenljivo magnetno polje, ki inducira električni tok v statorskem navitju.

Rotor je premikajoči del sinhronskega stroja in je lahko različne konstrukcije, odvisno od vrste stroja. Običajno ima rotor vzbujeno navitje, ki je napajano z zunanjim napajanjem . Ta vzbujeni rotor ustvari magnetno polje, ki je sinhronizirano z vrtenjem rotorja in omogoča prenos magnetne indukcije iz rotorja v stator. 

Ko rotor vrti magnetno polje znotraj statorja, se ustvarja sprememba magnetnega toka (fluksa) $\Phi$ skozi statorska navitja, kar inducira napetost $E_{2}$. Sinhronski stroj deluje v sinhronem načinu, kar pomeni, da se hitrost vrtenja rotorja ujema z frekvenco napetosti, ki se generira v statorskem navitju. Tako je frekvenca izhodne napetosti odvisna od hitrosti vrtenja, in število polov/polovih parov. Frekvenca se tako izračuna: 
$$f = p \frac{n}{60}$$
kjer je $p$ število polovih parov (na spodnji risbi sta dva pola in en polov par) in $n$ hitrost vrtenja rotorja v vrtljajih na minuto$\left[ \frac{vrt}{min} \right]$.

![[Sinhronski stroji 2024-11-30 10.45.07.excalidraw]]
## Trifazni dvopolni sinhronski stroj
Pri tej izvedbi sinhronskega stroja, imamo 3 tuljave na statorju. Ker so razporejene enakomirno, lahko rečemo da je njun geometrijski kot 120°, njun električni kot, je pa odvisen od števila polovih parov. V našem primeru je to samo en, zato je geometrijski kot enak električnemu.
![[Sinhronski stroji 2024-11-30 12.58.55.excalidraw]]
# Konstrukcija rotorja
Rotor je lahko sestavljen iz izraženimi poli ali iz cilindričnega rotorja. Razlika je v tem, da v izraženimi poli, je izražena tudi reluktanca, kar pomaga pri dodajanju navora. Ko je rotor cilindričen je zračna reža ves čas enaka. Navitje je malo posebno.

Rotor z izraženimi poli je možno realizirati z mnogimi poli, medtem ko clilindrični rotor ima lahko samo dva pola. 

Rotor vzbujamo z enosmernim tokom, da dobimo statičo magnetno polje. Rotacija rotorja je tista ki spreminja fluks ki ga vidi navitje statorja.

%% TODO: Nariši kontrukcijo rotorja cilindrične izvedbe. %%

# Konstrukcija statorja
