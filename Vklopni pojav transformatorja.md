---
related:
  - "[[Transformatorji]]"
tags:
  - unfinished
aliases:
  - predavanje 4
  - 
---
# Pojav
Ob vklopu stikala ob času $t_{0}$ steče tok $I_{1}$. če bi se ta spremenil hipno, bi se tudi magnetno polje $B$ spremenilo hipno. Če bi bilo to res, bi se na sekundarni strani inducirala neskončna napetost $E_{2} \to \infty$, saj velja $e_{i} = \frac{d\Phi}{dt} = A\frac{dB}{dt}$, kar bi pomenilo, da deljimo z 0, vemo pa, da je magnetno polje odvisno od toka skozi navitje.

Ker napetost ne more biti neskončna, imamo prehodni pojav. Na primarni strani se napetost spremeni hipoma, tok se pa ne more, zaradi reaktance navitja. 

Na sekundarni strani imamo odprte sponke in napajalna napetost je enosmerna.

![[Vklopni pojav transformatorja 2024-11-16 12.08.08.excalidraw]]
# Vpliv nelinearnosti jedra na preklopni pojav
Ker pred vklopom stikala $S$ ni v jedru nobenega magnetnega polja, je fluks ob času $t_{0}$ enak nič. V normalnem obratovalnem stanju fluks niha okoli osi $x$, vendar pri vklopu se premakne navzgor, tako kot je vidno na spodnjem grafu. To je zato, da lahko začne ob času $t_{0}$ z vrednostjo nič. Čez čas se vrne v normalno stanje.
![[Vklopni pojav transformatorja 2024-11-16 12.49.57.excalidraw]]
Sedaj ko razumemo kako se spreminja fluks ob vklopnem pojavu, lahko razumemo kako se spreminja tok:
![[Vklopni pojav transformatorja 2024-11-16 13.39.31.excalidraw]]
Krivulja toka naj bi zgledala podobno kot:
$$
\tanh^{-1}(0.95\sin(x))
$$
$i(t) = ?$, $N*i(t) = H(t)$, $B(t) = \frac{U}{4.44 f N A}$, $B(H) = B_{sat} \cdot \tanh\left( \frac{H}{H_{sat}} \right) \approx 1.6 \tanh\left( \frac{H}{1000} \right)$, $U = U_{max}\sin(2\pi \cdot 50\cdot t)$, $U_{max} = 230 V$, $N = 1000$, $A = 0.01$

# Po vklopnem pojavu
Ko vklopni pojav izveni zgleda stanje v transformatorju tako:
![[Vklopni pojav transformatorja 2024-11-16 12.27.07.excalidraw]]