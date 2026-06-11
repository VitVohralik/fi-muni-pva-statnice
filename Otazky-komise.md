# Přepis otázek od zkušební komise

---
# Teoretické základy informatiky a matematika
---
## 1. Lineární algebra

**1.** Co je vektor, vektorový prostor, axiomy vektorového prostoru?
> **Vektor** je prvek vektorového prostoru (uspořádaná $n$-tice čísel, geometricky šipka se směrem a velikostí). **Vektorový prostor** je množina $V$ s operacemi sčítání vektorů a násobení skalárem (z tělesa, např. $\mathbb{R}$), splňující axiomy: sčítání je asociativní a komutativní, má nulový vektor a ke každému vektoru opačný; násobení skalárem je distributivní (vůči součtu vektorů i skalárů), asociativní a platí $1 \cdot v = v$.

**2.** Co je matice, jak souvisí s lineární transformací a jaké další využití má?
> Obdélníkové schéma čísel ($m \times n$). Reprezentuje **lineární transformaci** (zobrazení mezi vektorovými prostory), zápis **soustavy lineárních rovnic**, dále data, grafy (matice sousednosti), rotace a projekce v grafice.

**3.** Operace s vektory a maticemi – skalární součin a jeho vlastnosti, vektorový součin.
> **Skalární součin** $u \cdot v = \sum u_i v_i$ (výsledkem je číslo) – komutativní, distributivní, lineární v každé složce. **Vektorový součin** (jen v $\mathbb{R}^3$) dává vektor kolmý na oba, jeho velikost = obsah rovnoběžníku.

**4.** Geometrický význam skalárního součinu, úhel svíraný vektory – vzorec.
> $u \cdot v = |u| \cdot |v| \cdot \cos\varphi$, kde $\varphi$ je úhel mezi vektory. Z toho $\cos\varphi = \dfrac{u \cdot v}{|u| \cdot |v|}$. Platí $u \cdot v = 0 \iff$ vektory jsou kolmé.

**5.** Násobení matic – příklad.
> Prvek $(i,j)$ výsledku = skalární součin $i$-tého řádku první matice a $j$-tého sloupce druhé. Násobit lze jen $A_{(m \times n)} \cdot B_{(n \times p)} = C_{(m \times p)}$; **není komutativní**. Příklad: $\begin{bmatrix}1&2\\3&4\end{bmatrix}\begin{bmatrix}5&6\\7&8\end{bmatrix} = \begin{bmatrix}19&22\\43&50\end{bmatrix}$.

**6.** Gaussova eliminační metoda – k čemu je, jak se rozepisuje, řešení soustav (co znamená řádek $0=1$?).
> Úprava matice na schodovitý (trojúhelníkový) tvar elementárními řádkovými úpravami. Slouží k řešení soustav, výpočtu hodnosti, inverze, determinantu a zjištění lineární (ne)závislosti. Řádek tvaru $0 = 1$ (vlevo samé nuly, vpravo nenula) znamená **spor → soustava nemá řešení**; řádek $0 = 0$ je nadbytečná rovnice (nekonečně mnoho řešení).

**7.** Determinant – jak se počítá, rozvoj podle prvního řádku, geometrický význam.
> Číslo přiřazené čtvercové matici. Pro $2 \times 2$: $ad - bc$; obecně **Laplaceův rozvoj** podle řádku/sloupce nebo přes trojúhelníkový tvar (součin diagonály). Geometricky $|\det|$ = obsah (2D) / objem (3D) rovnoběžníku nataženého na sloupcové vektory. $\det = 0 \iff$ vektory lineárně závislé $\iff$ matice není invertovatelná.

**8.** Vlastní čísla a vektory – co to je, jak se počítají, geometrický význam.
> Vlastní vektor $v$ matice $A$ je nenulový vektor, který se transformací jen škáluje: $A v = \lambda v$, kde $\lambda$ je vlastní číslo. Počítají se z **charakteristické rovnice** $\det(A - \lambda I) = 0$. Geometricky jsou to směry, které transformace nemění (jen prodlouží/zkrátí $\lambda$-krát). Využití: PCA, stabilita, PageRank.

**9.** Inverzní matice.
> $A^{-1}$ splňuje $A A^{-1} = A^{-1} A = I$. Existuje právě tehdy, je-li matice **čtvercová a regulární** ($\det \neq 0$, plná hodnost). Výpočet Gaussovou eliminací $[A \mid I] \to [I \mid A^{-1}]$. Řeší soustavu $Ax = b$ jako $x = A^{-1}b$.

**10.** Lineárně závislé/nezávislé vektory – definice, jak zjistit.
> Vektory jsou **lineárně nezávislé**, pokud jejich jediná lineární kombinace dávající nulový vektor má všechny koeficienty nulové. Zjištění: vektory dáme do matice, Gaussovou eliminací na horní trojúhelníkový tvar – počet nenulových řádků = počet nezávislých vektorů (hodnost).

**11.** Vektorové podprostory, báze – souřadnice vektoru, vztah k nezávislosti bázických vektorů.
> **Podprostor** je podmnožina uzavřená na sčítání a násobení skalárem. **Báze** je lineárně nezávislá množina vektorů, která generuje celý prostor; její velikost = dimenze. Souřadnice vektoru = koeficienty jeho vyjádření v bázi; bázické vektory musí být lineárně nezávislé.

**12.** Lineární obal, lineární kombinace.
> **Lineární kombinace** = výraz $a_1 v_1 + \dots + a_n v_n$. **Lineární obal** = množina všech lineárních kombinací daných vektorů (jimi generovaný podprostor).

**13.** Lineární transformace – co to je, vztah k maticím, definice.
> Zobrazení $f$ mezi vektorovými prostory zachovávající lineární strukturu: $f(u + v) = f(u) + f(v)$ a $f(a u) = a f(u)$. Každou lze v konečné dimenzi zapsat **maticí zobrazení**; aplikace = násobení vektoru touto maticí, její sloupce = obrazy bázových vektorů.

**14.** Matice rotace – jak vypadá, příklad rotace o 90°.
> Rotace o úhel $\varphi$: $\begin{bmatrix}\cos\varphi & -\sin\varphi\\ \sin\varphi & \cos\varphi\end{bmatrix}$. Pro 90°: $\begin{bmatrix}0 & -1\\ 1 & 0\end{bmatrix}$, takže bod $(x,y) \to (-y, x)$. Je to ortogonální matice ($\det = 1$, zachovává délky a úhly).

**15.** Jak reprezentujeme vektory v matici?
> Po souřadnicích – jako **řádky nebo sloupce** matice (dle konvence).

---

## 2. Základy matematické analýzy

**1.** Co je relace? (definice jako podmnožina kartézského součinu)
> Binární relace je libovolná **podmnožina kartézského součinu** $A \times B$ (množina uspořádaných dvojic). Obecně $n$-ární relace $\subseteq A_1 \times \dots \times A_n$.

**2.** Co je zobrazení/funkce, totální funkce, $n$-ární relace a zobrazení.
> **Funkce** je relace, která každému prvku definičního oboru přiřadí **nejvýše jeden** prvek oboru hodnot. **Totální funkce** přiřadí každému prvku **právě jeden** (je definovaná všude); jinak je parciální.

**3.** Vlastnosti reálných funkcí.
> Monotonie (rostoucí/klesající), ohraničenost (shora/zdola), parita (sudá $f(-x)=f(x)$, lichá $f(-x)=-f(x)$), prostota (injektivita), periodičnost, spojitost; definiční obor a obor hodnot. Polynom = $a_n x^n + \dots + a_1 x + a_0$, stupeň = nejvyšší mocnina.

**4.** Co znamená, že je funkce spojitá? (formální definice)
> $f$ je spojitá v bodě $a$, pokud $\lim_{x \to a} f(x) = f(a)$. Epsilon-delta: $\forall \varepsilon > 0\ \exists \delta > 0: |x - a| < \delta \Rightarrow |f(x) - f(a)| < \varepsilon$. Intuitivně: graf lze nakreslit jedním tahem bez zvednutí tužky.

**5.** Limita – formální definice (epsilon-delta), geometrický význam.
> $\lim_{x \to a} f(x) = L$: $\forall \varepsilon > 0\ \exists \delta > 0: 0 < |x - a| < \delta \Rightarrow |f(x) - L| < \varepsilon$. Geometricky: ať zvolíme jakkoli úzký pás $\pm\varepsilon$ kolem $L$, existuje okolí $\pm\delta$ kolem $a$, kde graf v pásu zůstává. Popisuje chování funkce v okolí bodu, ne nutně v bodě samém.

**6.** Derivace.
> $f'(a) = \lim_{h \to 0} \dfrac{f(a+h) - f(a)}{h}$ – okamžitá rychlost změny. Geometricky směrnice tečny ke grafu. $f' > 0$ → roste, $f' < 0$ → klesá, $f' = 0$ → kandidát na extrém. Např. $(x^n)' = n x^{n-1}$, $(\sin x)' = \cos x$.

**7.** Neurčitý a určitý integrál – jak se píše, geometrický význam, příklad kde je integrál nula (sinus).
> **Neurčitý** $\int f(x)\,dx = F(x) + C$ – množina primitivních funkcí ($F' = f$). **Určitý** $\int_a^b f(x)\,dx = F(b) - F(a)$ (Newton–Leibniz) – číslo, **obsah orientované plochy** mezi grafem a osou $x$ (nad osou $+$, pod osou $-$). Příklad nuly: $\int_0^{2\pi} \sin x\,dx = 0$ (kladná a záporná část se vyruší).

**8.** Diferenciální počet / diferenciální rovnice.
> **Diferenciální počet** studuje derivace a jejich aplikace (extrémy, průběh, aproximace). **Diferenciální rovnice** svazuje neznámou funkci s jejími derivacemi; řešením je funkce (ne číslo), např. $y' = y$ má řešení $y = C e^x$. Popisuje dynamické děje (růst, pohyb, ochlazování).

---

## Kombinatorika a pravděpodobnost

> *Není samostatnou otázkou v `Otazky.md`, ale látka pravděpodobnosti se prolíná s [[#3. Popisná statistika|Popisnou statistikou]].*

**1.** Kombinace bez opakování a s opakováním – definice, výpočet, kombinační číslo; proč je u kombinací s opakováním vzorec takový, jaký je.
> **Kombinace bez opakování** = výběr $k$ prvků z $n$ **bez ohledu na pořadí**: $\binom{n}{k} = \dfrac{n!}{k!(n-k)!}$ (kombinační číslo). **S opakováním** (prvky lze brát vícekrát): $\binom{n+k-1}{k}$. Vzorec je takový proto, že výběr $k$ prvků z $n$ typů s opakováním odpovídá rozmístění $k$ stejných kuliček do $n$ přihrádek (metoda „hvězd a přepážek": $k$ hvězd + $n-1$ přepážek, vybíráme jejich pozice).

**2.** Permutace bez opakování – definice, výpočet.
> Uspořádání všech $n$ prvků do pořadí: $P(n) = n!$. (Permutace s opakováním, kde se prvek opakuje $n_1, \dots, n_r$ krát: $\dfrac{n!}{n_1!\cdots n_r!}$.)

**3.** Variace s opakováním – definice, výpočet; rozdíl mezi kombinací a variací.
> **Variace** = výběr $k$ prvků z $n$, **kde záleží na pořadí**. Bez opakování $\dfrac{n!}{(n-k)!}$, **s opakováním** $n^k$. Rozdíl: u **variace záleží na pořadí**, u **kombinace ne**.

**4.** Pravidlo součtu a součinu.
> **Pravidlo součtu**: lze-li úlohu A udělat $m$ způsoby a (vzájemně se vylučující) úlohu B $n$ způsoby, je celkem $m+n$ možností. **Pravidlo součinu**: následuje-li po volbě s $m$ možnostmi volba s $n$ možnostmi, je celkem $m \cdot n$ možností.

**5.** Princip inkluze a exkluze.
> $|A \cup B| = |A| + |B| - |A \cap B|$; pro tři množiny $|A\cup B\cup C| = |A|+|B|+|C| - |A\cap B| - |A\cap C| - |B\cap C| + |A\cap B\cap C|$. Obecně se velikosti průniků **střídavě přičítají a odečítají**, aby se vícenásobně započtené prvky započítaly právě jednou.

**6.** Pravděpodobnost – definice, pravděpodobnostní pole/prostor elementárních jevů, jevový prostor.
> **Pravděpodobnostní prostor** $(\Omega, \mathcal{F}, P)$: $\Omega$ = prostor **elementárních jevů** (všechny možné výsledky), $\mathcal{F}$ = **jevové pole** (množina jevů $\subseteq \Omega$), $P$ = pravděpodobnostní míra. **Klasická (Laplaceova) definice**: $P(A) = \dfrac{|A|}{|\Omega|}$ (příznivé / všechny, při stejně pravděpodobných výsledcích). Axiomy: $P(A)\ge0$, $P(\Omega)=1$, σ-aditivita.

**7.** Podmíněná pravděpodobnost – definice.
> Pravděpodobnost jevu $A$ za podmínky, že nastal $B$: $P(A \mid B) = \dfrac{P(A \cap B)}{P(B)}$ (pro $P(B) > 0$). Jevy jsou **nezávislé**, když $P(A \cap B) = P(A)P(B)$, tedy $P(A\mid B) = P(A)$.

**8.** Bayesova věta – odvodit, uvést příklad využití.
> Z $P(A\mid B)P(B) = P(A\cap B) = P(B\mid A)P(A)$ plyne **Bayesova věta**: $P(A \mid B) = \dfrac{P(B \mid A)\,P(A)}{P(B)}$. Umožňuje „obrátit" podmíněnost. Příklad: z pozitivního výsledku testu ($B$) usoudit pravděpodobnost nemoci ($A$) při znalosti citlivosti testu a prevalence nemoci.

**9.** Příklad: hod dvěma kostkami – pravděpodobnost sudého čísla na druhé kostce, když na první padla 4.
> Hody jsou **nezávislé** – výsledek první kostky neovlivní druhou. Pravděpodobnost sudého čísla na druhé kostce je $\dfrac{3}{6} = \dfrac{1}{2}$ bez ohledu na to, že na první padla 4.

**10.** Spojitá pravděpodobnostní funkce.
> U spojité náhodné veličiny je pravděpodobnost popsána **hustotou** $f(x) \ge 0$ s $\int_{-\infty}^{\infty} f(x)\,dx = 1$; pak $P(a \le X \le b) = \int_a^b f(x)\,dx$ (obsah pod křivkou). Pravděpodobnost jednoho bodu je 0. Souvisí s distribuční funkcí $F(x) = \int_{-\infty}^x f(t)\,dt$ (viz Popisná statistika).

---

## 3. Popisná statistika

**1.** Střední hodnota – definice, co znamená, příklad na výpočet.
> Aritmetický průměr $\bar{x} = \frac{1}{n}\sum x_i$; pro náhodnou veličinu $E[X] = \sum x_i P(x_i)$. Vyjadřuje „těžiště" dat / očekávanou hodnotu, je **citlivá na odlehlé hodnoty**. Příklad: průměr z $\{2,4,9\} = 5$.

**2.** Medián.
> Prostřední hodnota seřazených dat (u sudého počtu průměr dvou prostředních), 50% kvantil. **Odolný vůči odlehlým hodnotám**. Příklad: medián z $\{1, 2, 100\} = 2$ (zatímco průměr $\approx 34{,}3$ je zkreslený).

**3.** Rozptyl – příklad na výpočet.
> $\sigma^2 = \frac{1}{n}\sum (x_i - \bar{x})^2$ – průměr kvadrátů odchylek od střední hodnoty, měří variabilitu. **Směrodatná odchylka** $\sigma = \sqrt{\sigma^2}$. Příklad pro $\{2,4,6\}$, $\bar{x}=4$: $\sigma^2 = \frac{4+0+4}{3} \approx 2{,}67$.

**4.** Korelace – jakou hodnotu by měla nakreslená data.
> Míra lineárního vztahu, koeficient $r \in \langle -1, 1\rangle$. $r=1$ dokonalá rostoucí lineární závislost, $r=-1$ klesající, $r=0$ žádná lineární závislost (náhodný mrak bodů). Korelace $\neq$ kauzalita, nezachytí nelineární vztahy.

**5.** Proč se normální rozdělení jmenuje „normální"?
> Protože **přirozeně vzniká** všude, kde se sčítá mnoho malých nezávislých vlivů (**centrální limitní věta**) – je to „normální/typický" stav. Gaussova křivka = symetrický zvon kolem $\mu$, šířka daná $\sigma$, pravidlo $68{-}95{-}99{,}7\,\%$.

**6.** Distribuční funkce – definice, nakreslit pro diskrétní a spojitou.
> $F(x) = P(X \le x)$ – pravděpodobnost, že veličina nepřekročí $x$. Je **neklesající**, **zprava spojitá**, jde od 0 do 1. U diskrétní veličiny je **schodovitá**, u spojité **hladká**.

**7.** Funkce hustoty pravděpodobnosti – co to je, vztah k distribuční funkci (derivace).
> Hustota $f(x)$ (spojitá veličina) je **derivace distribuční funkce** ($F'(x) = f(x)$). Pravděpodobnost = obsah pod hustotou na intervalu, celkový obsah $= 1$.

**8.** Nakreslit distribuční funkci rovnoměrného diskrétního rozložení a Gaussova rozložení.
> Rovnoměrné diskrétní (např. kostka) → **schodovitá** funkce s rovnoměrnými skoky $\frac{1}{6}$. Gaussovo → hladká **S-křivka (sigmoida)** rostoucí od 0 do 1, nejstrmější v $\mu$.

**9.** Nakreslit distribuční funkci rozložení, které na $(0,1)$ nabývá spojitou pravděpodobnost 0,5 a pro hodnotu 4 zbývajících 0,5.
> Smíšené rozdělení: na $(0,1)$ roste **lineárně** z 0 na 0,5 (rovnoměrná hustota na tomto intervalu), pak je konstantní na 0,5 až do $x=4$, kde má **skok** o 0,5 na hodnotu 1 (diskrétní atom v bodě 4).

**10.** Nakreslit distribuční funkci, která v 0 nabývá 0,5 a na intervalu $1$–$2$ je uniformní.
> Skok o 0,5 v bodě $x=0$ (diskrétní atom), pak konstanta 0,5 do $x=1$, na $\langle 1,2\rangle$ **lineární** růst z 0,5 na 1, dále konstanta 1.

**11.** Binomické rozložení – příklad na výpočet.
> Počet úspěchů v $n$ nezávislých pokusech: $P(k) = \binom{n}{k} p^k (1-p)^{n-k}$. Příklad: 3 hody mincí, $P(\text{2 hlavy}) = \binom{3}{2} (0{,}5)^2 (0{,}5)^1 = 3 \cdot 0{,}125 = 0{,}375$.

**12.** Rozdělení náhodných veličin a jejich příklady; odhady statistik a spolehlivost.
> **Diskrétní**: binomické, Poissonovo, rovnoměrné (kostka). **Spojité**: normální (Gaussovo), rovnoměrné, exponenciální. **Odhad** parametrů populace z výběru: bodový (jediná hodnota) vs intervalový (interval spolehlivosti, např. 95 %). Větší vzorek → užší interval, vyšší spolehlivost.

---

## Elementární teorie čísel

> *Není samostatnou otázkou v `Otazky.md`, ale vlastnosti relací se objevují u relací obecně a RSA/faktorizace u [[#10. Základy informační bezpečnosti|Informační bezpečnosti]].*

**1.** Dělitelnost – definice, relace (reflexivní, symetrická, antisymetrická, tranzitivní – dokázat).
> $a \mid b$ („$a$ dělí $b$") znamená $\exists k \in \mathbb{Z}: b = a \cdot k$. Relace dělitelnosti na $\mathbb{N}$ je:
> - **reflexivní**: $a \mid a$ (neboť $a = a\cdot 1$);
> - **antisymetrická**: $a\mid b \land b\mid a \Rightarrow a=b$ (na $\mathbb{N}$);
> - **tranzitivní**: $a\mid b \land b\mid c \Rightarrow a\mid c$ (z $b=ak$, $c=bl$ plyne $c = a(kl)$).
>
> **Není symetrická** (např. $2\mid 4$, ale $4\nmid 2$). Jde tedy o **částečné uspořádání**.

**2.** Euklidův algoritmus – příklad + pseudokód, PROČ funguje (invariant cyklu).
> Hledá $\gcd(a,b)$ opakovaným zbytkem: `while b != 0: (a, b) = (b, a mod b); return a`. Příklad $\gcd(48,18)$: $48 \bmod 18 = 12$, $18 \bmod 12 = 6$, $12 \bmod 6 = 0 \Rightarrow$ **6**. **Funguje** díky invariantu $\gcd(a,b) = \gcd(b, a \bmod b)$ – společní dělitelé $a,b$ jsou totožní se společnými děliteli $b$ a $a \bmod b$; zbytek se v každém kroku zmenšuje, proto algoritmus skončí.

**3.** Modulární operace – jak poznáme, hlavně dělení (zlomek mod přirozené číslo – příklad).
> $a \bmod n$ = zbytek po dělení. Sčítání, odčítání i násobení mod $n$ fungují přímo. **Dělení** mod $n$ není obyčejné – znamená násobení **multiplikativní inverzí**: $a/b \bmod n = a \cdot b^{-1} \bmod n$, kde $b^{-1}$ existuje **jen když** $\gcd(b,n)=1$ (najde se rozšířeným Euklidovým algoritmem). Příklad $1/3 \bmod 7$: $3^{-1} \equiv 5$ (protože $3\cdot5=15\equiv1$), takže $1/3 \equiv 5 \pmod 7$.

**4.** Prvočísla – definice prvočísla a složeného čísla, kolik existuje prvočísel.
> **Prvočíslo** = přirozené číslo $> 1$ dělitelné jen 1 a sebou samým; **složené** má i jiného dělitele. Prvočísel je **nekonečně mnoho** (Euklidův důkaz sporem: kdyby jich bylo konečně $p_1,\dots,p_k$, číslo $p_1\cdots p_k + 1$ není dělitelné žádným z nich → spor).

**5.** Základní věta aritmetiky, faktorizace na prvočísla (je rozklad jednoznačný?).
> **Každé přirozené číslo $> 1$ lze zapsat jako součin prvočísel, a to jednoznačně až na pořadí** (prvočíselný rozklad). Rozklad je tedy **jednoznačný**. Faktorizace velkých čísel je výpočetně těžká – na tom stojí RSA.

**6.** Testování prvočíselnosti – hrubá síla, Fermatův test (proč je lepší – mocnění je rychlejší než dělení), Eratosthenovo síto.
> **Hrubá síla**: zkoušíme dělitele do $\sqrt{n}$. **Fermatův test** (pravděpodobnostní): využívá **Malou Fermatovu větu** $a^{p-1} \equiv 1 \pmod p$ pro prvočíslo $p$; je rychlejší, protože **modulární mocnění** (square-and-multiply) je rychlejší než zkoušení mnoha dělení – ale existují Carmichaelova čísla, která ho oklamou (řeší Miller-Rabin). **Eratosthenovo síto** najde všechna prvočísla do $N$ vyškrtáním násobků.

**7.** Jak generovat velká prvočísla (tvar $2^n - 1$).
> Náhodně se zvolí velké liché číslo a otestuje pravděpodobnostním testem (Fermat/Miller-Rabin); neprojde-li, zkusí se další. **Mersennova prvočísla** mají tvar $2^n - 1$ (nutná podmínka: $n$ samo prvočíslo) – pro ně existuje efektivní Lucas–Lehmerův test, proto jsou mezi největšími známými prvočísly.

**8.** Jak se mocní velká čísla.
> **Rychlým mocněním (square-and-multiply)**: $a^e$ se spočítá opakovaným umocňováním na druhou podle binárního zápisu exponentu – místo $e$ násobení stačí $O(\log e)$. V kryptografii vždy **modulárně** ($a^e \bmod n$), aby čísla nerostla.

**9.** RSA – celý algoritmus (generování klíčů, šifrování, dešifrování), proč je bezpečné (faktorizace), Eulerova věta.
> **Generování klíčů**: zvol prvočísla $p,q$; $n=pq$; $\varphi(n)=(p-1)(q-1)$; zvol $e$ nesoudělné s $\varphi(n)$; spočti $d = e^{-1}\bmod\varphi(n)$. Veřejný klíč $(e,n)$, soukromý $(d,n)$. **Šifrování** $c=m^e\bmod n$, **dešifrování** $m=c^d\bmod n$. Funguje díky **Eulerově větě** $m^{\varphi(n)}\equiv1\pmod n$, takže $m^{ed}=m^{1+k\varphi(n)}\equiv m$. **Bezpečnost** stojí na obtížnosti **faktorizace** $n$ (z ní by šlo dopočítat $\varphi(n)$ a $d$).

**10.** Eulerova funkce – je snadno vypočitatelná?
> $\varphi(n)$ = počet čísel $\le n$ nesoudělných s $n$. **Snadno vypočitatelná jen při znalosti prvočíselného rozkladu**: $\varphi(n) = n\prod_{p\mid n}\!\left(1-\tfrac1p\right)$; pro $n=pq$ je $\varphi(n)=(p-1)(q-1)$. Bez znalosti faktorizace je výpočet $\varphi(n)$ stejně těžký jako faktorizace – proto je RSA bezpečné.

**11.** Podepisování zpráv pomocí RSA.
> Podpis = **opačné použití klíčů**: odesílatel zašifruje **haš** zprávy svým **soukromým** klíčem $s = h(m)^d \bmod n$; kdokoli ověří **veřejným** klíčem $s^e \bmod n \stackrel{?}{=} h(m)$. Zaručuje autenticitu, integritu a nepopiratelnost.

---

## 4. Grafy a jejich prohledávání

**1.** Co je graf? (formální definice)
> $G = (V, E)$, kde $V$ je množina vrcholů a $E$ množina hran. **Neorientovaný**: hrany jsou dvouprvkové množiny $\{u,v\}$; **orientovaný**: hrany jsou uspořádané dvojice $(u,v)$ se směrem. Hrana může mít ohodnocení (váhu).

**2.** Typy grafů – orientované, neorientované, rovinný graf, klika.
> Orientovaný/neorientovaný, ohodnocený, souvislý, **rovinný (planární)** = lze nakreslit do roviny bez křížení hran, **úplný graf / klika** = každé dva vrcholy spojeny hranou, strom, bipartitní, DAG.

**3.** Stromy – definice kořene v orientovaném a neorientovaném stromu.
> Strom = souvislý acyklický neorientovaný graf ($n-1$ hran). V **neorientovaném** stromu lze kořen zvolit libovolně (zakořenění); v **orientovaném** je kořen vrchol se **vstupním stupněm 0**, z něhož vedou cesty ke všem ostatním. Listy = vrcholy bez potomků.

**4.** Stupně vrcholů.
> Počet hran incidentních s vrcholem. U orientovaného grafu rozlišujeme **vstupní** (in-degree) a **výstupní** (out-degree). Princip sudosti: $\sum \deg(v) = 2|E|$ (každá hrana přispěje 2).

**5.** Reprezentace grafů – matice sousednosti, seznam následníků (výhody/nevýhody, složitosti, řídké vs husté).
> **Matice sousednosti** ($V \times V$): test hrany $O(1)$, paměť $O(V^2)$ – pro **husté** grafy. **Seznam následníků**: paměť $O(V+E)$, rychlý průchod sousedů, pomalejší test konkrétní hrany – pro **řídké** grafy.

**6.** DFS – jak funguje, obarvování vrcholů, post-order DFS, využití.
> Jde co nejhlouběji, pak se vrací (backtracking); zásobník / rekurze. **Obarvuje vrcholy** (bílá/šedá/černá) → detekce cyklů (hrana do šedého). **Post-order** se využívá k topologickému řazení a hledání silně souvislých komponent. Složitost $O(V+E)$.

**7.** BFS – jak funguje, datová struktura, lze použít na hledání cyklů?
> Prochází graf po vrstvách, používá **frontu (FIFO)**. Najde **nejkratší cestu v neohodnoceném grafu** (nejmenší počet hran). Lze použít i na detekci cyklů a test souvislosti/bipartitnosti. Složitost $O(V+E)$.

**8.** Komponenty souvislosti – definice (formálně přes relaci).
> Maximální souvislé podgrafy. Formálně přes **relaci dosažitelnosti** „existuje cesta mezi $u$ a $v$" – ta je reflexivní, symetrická a tranzitivní (ekvivalence) a její **třídy ekvivalence** jsou právě komponenty souvislosti. U orientovaných grafů rozlišujeme slabé a silné komponenty. Zjistíme opakovaným DFS/BFS.

---

## 5. Grafové algoritmy

**1.** Co je nejkratší cesta – formální definice, kdy existuje.
> Cesta mezi dvěma vrcholy s minimálním součtem vah hran. V neohodnoceném grafu = nejmenší počet hran (BFS). Existuje, je-li cíl **dosažitelný** z počátku; **není dobře definovaná**, leží-li na cestě **záporný cyklus** (délku lze snižovat donekonečna).

**2.** Co je cesta, sled, jednoduchá cesta?
> **Sled (walk)** – posloupnost vrcholů a hran, vrcholy i hrany se mohou opakovat. **Tah** – sled bez opakování hran. **Cesta (jednoduchá cesta)** – sled bez opakování **vrcholů**. Kružnice = uzavřená cesta.

**3.** Co je minimální kostra grafu – definice (minimální souvislý podgraf).
> **Kostra** = podgraf, který je stromem a obsahuje všechny vrcholy (souvislý, acyklický, $n-1$ hran). **Minimální kostra (MST)** má nejmenší součet vah hran. Definuje se pro souvislý ohodnocený neorientovaný graf. *(Pozn.: jde o minimální souvislý* ***podgraf, který spojuje všechny vrcholy*** *– kostra, ne libovolný podgraf.)*

**4.** Dijkstrův algoritmus – popis, příklad, omezení (jen nezáporné hrany), složitost a její odvození.
> Hledá nejkratší cesty z jednoho zdroje; hladově vybírá nejbližší nezpracovaný vrchol a relaxuje jeho hrany. **Omezení: jen nezáporné váhy**. Využívá prioritní frontu (haldu). Složitost $O((V+E)\log V)$ – každý vrchol vyjmut jednou, každá hrana jednou relaxována, operace haldy $\log V$.

**5.** Bellman-Fordův algoritmus – popis, omezení (nemá), co se stane při záporném cyklu (odhalí ho – jak?).
> Hledá nejkratší cesty i pro **záporné hrany**. Provede $V-1$ iterací, v každé relaxuje všechny hrany; složitost $O(V \cdot E)$. **Detekce záporného cyklu**: po $V-1$ iteracích se provede ještě jedna – pokud lze stále relaxovat, existuje záporný cyklus.

**6.** Rozdíl mezi Dijkstrou a Bellman-Fordem.
> Záporné hrany: jen Bellman-Ford; záporný cyklus odhalí jen Bellman-Ford. Složitost: Dijkstra $O((V+E)\log V)$ (rychlejší), BF $O(V \cdot E)$. Princip: Dijkstra hladový (prioritní fronta), BF dynamické programování (opakovaná relaxace).

**7.** Kde by Dijkstra selhal při přidání záporné hrany – ukázat na grafu.
> Dijkstra předpokládá, že „uzavřený" vrchol má finální vzdálenost. Příklad: $A \to B = 2$, $A \to C = 5$, $C \to B = -10$. Dijkstra uzavře $B$ s hodnotou 2, ale skutečná nejkratší cesta $A \to C \to B = -5$. K uzavřenému vrcholu se algoritmus nevrátí.

**8.** Jarník-Primův a Kruskalův algoritmus – popis a ukázka.
> **Jarník-Prim** roste jeden strom od počátečního vrcholu, přidává nejlevnější hranu ke stromu, prioritní fronta, $O((V+E)\log V)$, vhodný pro husté grafy. **Kruskal** bere hrany od nejlevnější a přidá je, pokud nevytvoří cyklus (test přes **Union-Find**), $O(E \log E)$, vhodný pro řídké grafy.

**9.** Jaký grafový algoritmus řeší NP-úplný problém?
> **Problém obchodního cestujícího (TSP)** – nejkratší okružní cesta přes všechny vrcholy. Související NP-úplné: Hamiltonovská kružnice, barvení grafu, největší klika, vrcholové pokrytí. Naopak nejkratší cesta a MST jsou v **P**.

---

## 6. Stromové datové struktury

**1.** Binární vyhledávací strom (BST) – co to je, jak se hledá, operace (insert, delete), složitosti, nejhorší případ, použití.
> Binární strom, kde pro každý uzel platí: levý podstrom menší klíče, pravý větší. Hledání/vkládání/mazání porovnáním klíče – $O(h)$. Vyvážený: $O(\log n)$; **nejhorší případ (degenerace na seznam): $O(n)$**. Inorder průchod vydá klíče seřazené. Použití: slovníky, množiny, indexy.

**2.** Problémy s BST → samovyvažovací stromy, rotace (znázornění, složitost).
> Při vkládání v nevhodném pořadí (seřazená data) BST degeneruje na lineární seznam → $O(n)$. **Samovyvažovací stromy** (AVL, červeno-černé) udržují hloubku $O(\log n)$. **Rotace** = lokální přestrukturování (levá/pravá) snižující výšku se zachováním uspořádání BST, složitost $O(1)$.

**3.** Hloubka stromu a vztah ke složitosti hledání.
> Složitost operací přímo odpovídá **hloubce** stromu ($O(h)$). Vyvážený strom má $h \in O(\log n)$, degenerovaný $h \in O(n)$.

**4.** Červeno-černé stromy – pravidla, insert (příklad s rotací a přebarvením), složitost operací.
> Samovyvažovací BST, každý uzel červený/černý: kořen černý, červený uzel nemá červeného potomka, každá cesta z uzlu do listů (NIL) má **stejný počet černých uzlů**. Výška $\le 2\log n$. Insert/delete/search v $O(\log n)$, vyvažování **rotacemi a přebarvováním**. Použití: `std::map`, `TreeMap`, plánovače v jádře.

**5.** B-stromy – co to je, pravidla (minimální stupeň větvení, počet klíčů, listy ve stejné hloubce), insert (vkládá se do listů), složitosti, použití (databáze, operace s diskem).
> Vyvážený vyhledávací strom s vysokým větvením. Parametr **minimální stupeň $t$**: každý uzel (kromě kořene) má $t-1$ až $2t-1$ klíčů; **všechny listy ve stejné hloubce**. Vkládá se do listů, při přeplnění se uzel **rozdělí (split)**. Operace $O(\log n)$ s malou výškou → málo přístupů na disk. Použití: databáze a souborové systémy (varianta B+ strom).

**6.** Halda – jak funguje, vlastnost (úplný binární strom kromě poslední vrstvy zarovnané doleva), operace + složitosti, implementace polem a proč, použití.
> Binární strom s vlastností haldy: rodič $\le$ (min-halda) / $\ge$ (max-halda) potomci. Je to **úplný binární strom** (poslední vrstva zarovnaná doleva), proto **implementace polem**: potomci uzlu $i$ jsou $2i+1$ a $2i+2$ – žádné ukazatele. Insert, extract-min/max v $O(\log n)$, čtení kořene $O(1)$. Použití: prioritní fronta (Dijkstra, Jarník-Prim), heapsort.

**7.** Přehled všech struktur – k čemu se které používají.
> **BST/červeno-černý** – slovník/množina v paměti, řazené iterování, $O(\log n)$. **B/B+ strom** – velká data na disku (DB, FS), minimalizace I/O. **Halda** – prioritní fronta, výběr min/max, heapsort. Pro pouhé vyhledávání bez řazení bývá rychlejší **hašovací tabulka** ($O(1)$ průměrně).

---

## 7. Návrh algoritmů

**1.** Co je metoda rozděl a panuj?
> Strategie ve třech krocích: **Rozděl** problém na menší podproblémy téhož typu, **Panuj** (vyřeš rekurzivně, triviální přímo), **Spoj** dílčí řešení. Příklady: merge sort, quick sort, binární vyhledávání. Složitost často přes master teorém.

**2.** Merge sort – jak funguje, jak se pole rozdělí, jak funguje merge, příklad, složitost $O(n\log n)$ – dokázat (rekurzivní strom, výška stromu).
> Pole rozdělí na dvě poloviny, každou rekurzivně seřadí, pak **slije (merge)** lineárním průchodem $O(n)$. **Důkaz $O(n\log n)$**: rekurzivní strom má výšku $\log n$ (půlení), na každé úrovni se spojuje celkem $O(n)$ prvků → $n \log n$. Stabilní, ale potřebuje $O(n)$ paměti navíc.

**3.** Quick sort – jak funguje, složitost.
> Zvolí **pivot**, rozdělí pole na menší/větší (partition), rekurzivně seřadí obě části. Průměrně $O(n\log n)$, in-place, v praxi rychlý. **Nejhorší případ $O(n^2)$** (špatná volba pivotu, např. seřazené pole s krajním pivotem) – řeší se náhodným/medián pivotem.

**4.** Pseudokód rekurzivního faktoriálu, iterativní faktoriál; jak funguje rekurze.
> Rekurze = funkce volá sebe na menším vstupu až do **bázového případu**. Rekurzivní: `fact(n) = if n<=1 then 1 else n*fact(n-1)`. Iterativní: `r=1; for i=2..n: r*=i; return r`. Každé volání má vlastní rámec na **zásobníku** (riziko přetečení).

**5.** Tail rekurze – je daný kód tail rekurzivní? Jak upravit na tail rekurzi.
> **Tail rekurze** = rekurzivní volání je úplně poslední operací (výsledek se dál neupravuje). Kompilátor ji přeloží na **cyklus** (TCO) bez růstu zásobníku. Faktoriál upravíme přidáním **akumulátoru**: `fact(n,acc) = if n<=1 then acc else fact(n-1, n*acc)`.

**6.** Výhody a nevýhody rekurze, odstranění rekurze.
> **Výhody**: čitelný kód pro rekurzivní strukturu (stromy, rozděl a panuj). **Nevýhody**: režie volání, přetečení zásobníku, opakované výpočty. **Odstranění**: převod na iteraci s explicitním zásobníkem, tail-call optimalizace, dynamické programování / memoizace.

**7.** Vztah rekurze a matematické indukce – indukce dokazuje správnost rekurzivních algoritmů.
> Dvě strany téže mince. **Indukce**: báze + indukční krok (z $n$ na $n+1$). **Rekurze**: bázový případ + rekurzivní krok (řešení z menších instancí). Proto se **korektnost rekurzivního algoritmu dokazuje indukcí** podle velikosti vstupu.

**8.** Napsat důkaz korektnosti rekurzivního algoritmu.
> Indukcí podle velikosti vstupu: (1) **báze** – ukáži správnost pro nejmenší případ; (2) **indukční krok** – za předpokladu korektnosti pro menší vstupy ukáži, že z korektních dílčích výsledků plyne korektní celek. (Iterativní algoritmus se dokazuje **invariantem cyklu**: inicializace, zachování, ukončení.)

---

## 8. Funkcionální programování

**1.** Princip výpočtu ve funkcionálním programování, rozdíl mezi imperativním a deklarativním přístupem.
> **Imperativní** popisuje **JAK** (posloupnost příkazů měnících stav). **Deklarativní/funkcionální** popisuje **CO** se má spočítat (vyhodnocování výrazů, žádný měnitelný stav). Výpočet = **postupná redukce výrazu** aplikací funkcí; funkce jsou čisté, data neměnná.

**2.** Redukční krok, redukční strategie – striktní (eager) a normální (lazy), rozdíl, příklad na výrazu.
> **Redukční krok** = nahrazení redexu podle definice funkce. **Striktní (eager, call-by-value)** – nejdřív vyhodnotí argumenty, pak aplikuje funkci. **Normální (leftmost-outermost, call-by-name)** – nejdřív aplikuje vnější funkci, argumenty až když jsou potřeba.

**3.** Vlastnosti strategií – příklad funkce, která se cyklí na striktní, ale ne na normální strategii.
> **Normální strategie je normalizující** – má-li výraz normální formu, najde ji; striktní nemusí. Příklad: `const x y = x`, `loop = loop`. Výraz `const 1 loop`: striktní se snaží vyhodnotit `loop` → **zacyklí**; normální rovnou vrátí `1`.

**4.** Nevýhoda normální strategie (dvojí vyhodnocení výrazů) → líné vyhodnocování v Haskellu.
> Nevýhoda: argument může být vyhodnocen **vícekrát** (použije-li se opakovaně). Řešení: **líné vyhodnocování** = normální strategie + **sdílení** (každý výraz se vyhodnotí nejvýše jednou, výsledek se zapamatuje). Používá Haskell; umožňuje nekonečné datové struktury.

**5.** Funkce vyšších řádů – co to jsou, příklad (`map`), implementovat `map` na tabuli včetně typu.
> Funkce, která bere funkci jako argument nebo ji vrací (`map`, `filter`, `fold`). V Haskellu:
> ```haskell
> map :: (a -> b) -> [a] -> [b]
> map _ []     = []
> map f (x:xs) = f x : map f xs
> ```

**6.** Nepojmenované (lambda) funkce.
> Funkce bez jména, definovaná „na místě". Haskell: `\x -> x + 1`. Užitečné jako argumenty funkcí vyšších řádů: `map (\x -> x*x) [1,2,3]` → `[1,4,9]`. Vychází z **lambda kalkulu** – teoretického základu FP.

**7.** Napsat program v Haskellu – nekonečný seznam jedniček; typy v Haskellu.
> Nekonečný seznam (díky lenosti): `ones = 1 : ones` nebo `ones = repeat 1`; bereme konečně: `take 5 ones` → `[1,1,1,1,1]`. Haskell je **silně a staticky typovaný** s odvozováním typů; zápis `f :: Int -> Int`, typové třídy (`Num`, `Eq`) umožňují polymorfismus.

---

## 9. Regulární jazyky

**1.** Chomského hierarchie – typy gramatik, pravidla pro dané jazyky, rozdíly mezi typy.
> Čtyři vnořené třídy: **Typ 0** rekurzivně spočetné (obecné gramatiky, Turingův stroj), **Typ 1** kontextové (kontextové gramatiky, lineárně omezený automat), **Typ 2** bezkontextové (pravidla $A \to \alpha$, zásobníkový automat), **Typ 3** regulární (pravidla $A \to aB$ / $A \to a$, konečný automat). Platí $\text{Typ 3} \subset \text{Typ 2} \subset \text{Typ 1} \subset \text{Typ 0}$.

**2.** Co je jazyk, co je gramatika – formální definice (uspořádaná čtveřice).
> **Abeceda $\Sigma$** = konečná množina symbolů, **slovo** = konečná posloupnost symbolů, **jazyk** = podmnožina $\Sigma^*$. **Gramatika $G = (N, \Sigma, P, S)$**: $N$ neterminály, $\Sigma$ terminály ($N \cap \Sigma = \emptyset$), $P$ přepisovací pravidla $\alpha \to \beta$, $S \in N$ počáteční symbol.

**3.** Regulární jazyky – definice, reprezentace (gramatiky, automaty, regulární výrazy), převody mezi nimi.
> Třída typu 3 – přesně jazyky **rozpoznatelné konečným automatem**. Tři ekvivalentní reprezentace: **konečné automaty** (DFA, NFA, NFA-ε), **regulární výrazy**, **regulární (pravé lineární) gramatiky**. Všechny popisují stejnou třídu a algoritmicky se převádějí (Kleeneova věta).

**4.** DFA – definice (uspořádaná pětice), přechodová funkce.
> $M = (Q, \Sigma, \delta, q_0, F)$: $Q$ stavy, $\Sigma$ abeceda, $\delta: Q \times \Sigma \to Q$ (z každého stavu na každý symbol **právě jeden** přechod), $q_0$ počáteční stav, $F \subseteq Q$ přijímající stavy. Slovo je přijato, skončí-li automat ve stavu z $F$.

**5.** NFA – definice; determinismus a nedeterminismus – vztah, rozdíl.
> NFA má $\delta: Q \times \Sigma \to \mathcal{P}(Q)$ (vrací **množinu stavů**, více možností nebo žádnou). Přijímá slovo, **existuje-li aspoň jedna** přijímající výpočetní cesta. DFA a NFA rozpoznávají **stejnou třídu** (regulární) – nedeterminismus zde nepřidává sílu, jen úspornost zápisu.

**6.** Determinizace NFA → DFA: kolik max vznikne stavů ($2^n$) + odůvodnění.
> **Podmnožinová konstrukce**: stavy DFA = množiny stavů NFA, proto až $2^n$ stavů (každá podmnožina $n$-prvkové množiny stavů). Počáteční stav = ε-uzávěr počátečního; přechod z $S$ na $a$ = ε-uzávěr sjednocení $\delta(q,a)$ pro $q \in S$; přijímající = množiny obsahující aspoň jeden přijímající stav NFA.

**7.** Nakreslit automat rozpoznávající lichý počet a-ček.
> Dvoustavový DFA: stav $q_0$ (sudý počet $a$, počáteční, nepřijímající) a $q_1$ (lichý počet $a$, přijímající). Na symbol $a$ se stavy přepínají ($q_0 \leftrightarrow q_1$), na ostatní symboly zůstávají (smyčka). Přijímá v $q_1$.

**8.** Převod DFA → regulární výraz (5stavový převod); z automatu vytvořit gramatiku.
> **DFA → reg. výraz**: metoda **eliminace stavů** – postupně odstraňujeme stavy a hrany přeznačujeme regulárními výrazy, až zbyde počáteční a koncový stav spojený jediným výrazem (lze i přes Ardenovo lemma). **Automat → gramatika**: stavy = neterminály, přechod $p \xrightarrow{a} q$ dá pravidlo $p \to aq$, pro přijímající stav přidáme $p \to \varepsilon$.

**9.** Uzávěrové vlastnosti regulárních jazyků – průnik, rozdíl, sjednocení, doplněk; nástin důkazu (produktový automat).
> Třída je uzavřená na sjednocení, průnik, doplněk (rozdíl), konkatenaci, iteraci, zrcadlový obraz, homomorfismus. Důkazy konstrukcí: doplněk = prohození přijímajících/nepřijímajících stavů v **úplném DFA**; průnik/sjednocení = **produktový (součinový) automat**.

**10.** Paralelní synchronní kompozice automatů – jak přesně funguje.
> Konstrukce **produktového automatu** simulujícího dva automaty zároveň: stavy = dvojice $(p,q)$, na vstupní symbol oba dělají přechod **synchronně**. Volbou přijímajících stavů získáme **průnik** (oba přijímají) nebo **sjednocení** (aspoň jeden). Základ důkazu uzávěrových vlastností na průnik a rozdíl.

---

## Bezkontextové jazyky a jejich reprezentace

> *Není samostatnou otázkou v `Otazky.md`, ale navazuje přímo na [[#9. Regulární jazyky|Regulární jazyky]] (Chomského hierarchie) a [[#10. Rozhodnutelnost|Rozhodnutelnost]].*

**1.** Zařazení do Chomského hierarchie.
> **Typ 2** Chomského hierarchie. Platí $\text{regulární (typ 3)} \subsetneq \text{bezkontextové (typ 2)} \subsetneq \text{kontextové (typ 1)}$. Rozpoznávají je **zásobníkové automaty (PDA)**.

**2.** Definice bezkontextové gramatiky, příklady pravidel.
> Gramatika $G=(N,\Sigma,P,S)$, kde každé pravidlo má tvar $A \to \alpha$ s **jedním neterminálem** $A \in N$ vlevo a $\alpha \in (N\cup\Sigma)^*$ vpravo (levá strana nezávisí na kontextu). Příklad: $S \to aSb \mid \varepsilon$ generuje $\{a^n b^n \mid n\ge0\}$.

**3.** Co je bezkontextový jazyk – generuje ho bezkontextová gramatika nebo PDA.
> Jazyk **generovaný nějakou bezkontextovou gramatikou** – ekvivalentně **rozpoznávaný zásobníkovým automatem**. Příklady: vyvážené závorky, $a^nb^n$, palindromy – jazyky vyžadující „počítání"/zanořování, které regulární automat nezvládne.

**4.** Zásobníkový automat (PDA) – definice, přechodová funkce, jak funguje (i intuitivně).
> Sedmice $(Q,\Sigma,\Gamma,\delta,q_0,Z_0,F)$: stavy, vstupní abeceda, **zásobníková abeceda** $\Gamma$, přechodová funkce, počáteční stav, počáteční symbol zásobníku, přijímající stavy. **Přechod** $\delta: Q\times(\Sigma\cup\{\varepsilon\})\times\Gamma \to \mathcal{P}(Q\times\Gamma^*)$ – podle stavu, vstupního symbolu a **vrcholu zásobníku** přejde do nového stavu a vrchol nahradí řetězcem. Intuitivně: konečný automat + **zásobník** jako neomezená pomocná paměť (LIFO).

**5.** Napsat krok výpočtu PDA.
> Konfigurace = (stav, zbytek vstupu, obsah zásobníku). Krok: $(q,\, aw,\, X\gamma) \vdash (q',\, w,\, \beta\gamma)$, pokud $(q',\beta) \in \delta(q,a,X)$ – přečte $a$, nahradí vrchol $X$ řetězcem $\beta$. Např. při čtení $a$ se symbol pushne, při čtení $b$ popne.

**6.** Metody akceptování PDA – akceptující stav, prázdný zásobník; musí být ε na vstupu při akceptování?
> Dvě **ekvivalentně silné** metody: přijetí **přijímajícím stavem** (po přečtení celého vstupu je automat v $F$) nebo **prázdným zásobníkem**. Při akceptování musí být **celý vstup přečten** (na vstupu zbývá $\varepsilon$); zásobník u akceptace stavem prázdný být nemusí.

**7.** Rozdíl mezi rozšířeným a normálním PDA; determinismus a nedeterminismus u PDA.
> **Normální PDA** v jednom kroku nahradí jen vrchol zásobníku; **rozšířený** smí přečíst/nahradit více symbolů zásobníku najednou – jsou ekvivalentně silné. **Nedeterministický PDA** rozpoznává **všechny** bezkontextové jazyky, ale **deterministický PDA** jen jejich vlastní podtřídu (deterministické BKJ) – nedeterminismus zde **přidává sílu** (na rozdíl od konečných automatů).

**8.** Navrhnout PDA akceptující $a^n b^{2n}$ a napsat gramatiku.
> **PDA**: pro každé přečtené $a$ pushni **dva** symboly (např. dvě $X$); pak pro každé $b$ popni jedno $X$; přijmi prázdným zásobníkem, sedí-li počty. **Gramatika**: $S \to aSbb \mid \varepsilon$ (každé $a$ přidá dvě $b$).

**9.** Nedeterministická syntaktická analýza – analýza zdola nahoru.
> **Syntaktická analýza (parsing)** hledá derivaci slova v gramatice. **Zdola nahoru (bottom-up)** začíná u terminálů vstupu a redukuje je podle pravidel zpět k počátečnímu symbolu $S$ (shift-reduce, např. LR). Obecná bezkontextová gramatika může být nejednoznačná → **nedeterministická** analýza zkouší více možností (backtracking, CYK, Earley).

**10.** Uzávěrové vlastnosti bezkontextových jazyků – co znamená uzavřenost na operaci.
> **Uzavřenost na operaci** = aplikací operace na bezkontextové jazyky vznikne opět bezkontextový jazyk. BKJ jsou uzavřené na **sjednocení, konkatenaci, iteraci (Kleene)**, ale **NEjsou** uzavřené na **průnik** ani **doplněk** (např. $a^nb^nc^n$ vznikne průnikem dvou BKJ a sám bezkontextový není).

**11.** Vadilo by dát epsilon krok kamkoliv? (ne)
> Ne. PDA smí provádět **ε-kroky** (přechod bez čtení vstupu, jen manipulace zásobníku) kdekoli – je z principu nedeterministický, takže přidání ε-přechodů nemění třídu rozpoznávaných jazyků (stále právě bezkontextové).

---

## 10. Rozhodnutelnost

**1.** Co je algoritmický problém – definice (vstup $x$, výstupní funkce $D(x)$).
> Přesně zadaná otázka pro nekonečně mnoho vstupů, často jako **rozhodovací problém** (odpověď ANO/NE), formálně **jazyk** = množina vstupů s odpovědí ANO. $D(x)$ je požadovaný výstup pro vstup $x$.

**2.** Co je algoritmus.
> Konečný, jednoznačný postup, který pro vstup po konečném počtu kroků vydá výsledek. **Church–Turingova teze**: pojem „algoritmus" je přesně zachycen Turingovým strojem.

**3.** Turingův stroj – definice (intuitivně i formálně jako sedmice), krok výpočtu, konfigurace, přechodová funkce.
> Abstraktní model s neomezenou **páskou** + čtecí/zápisová hlava, konečnou množinou stavů a **přechodovou funkcí** (stav, čtený symbol) → (nový stav, zapsaný symbol, posun L/R). **Krok výpočtu**: přečte symbol, přepíše, posune hlavu, změní stav. **Konfigurace** = úplný popis stavu výpočtu (stav řízení, obsah pásky, pozice hlavy). Formálně sedmice $(Q, \Sigma, \Gamma, \delta, q_0, q_{accept}, q_{reject})$.

**4.** K čemu je dobrý Turingův stroj.
> Slouží jako **formální definice algoritmu / vyčíslitelnosti** – vše, co je algoritmicky řešitelné, je řešitelné TS. Umožňuje přesně definovat rozhodnutelnost, složitostní třídy a dokazovat nerozhodnutelnost (diagonalizace, redukce).

**5.** Problém zastavení (HALT) – definice, je částečně rozhodnutelný, proč je nerozhodnutelný (diagonalizace – myšlenka důkazu).
> $\text{HALT} = \{\langle M, w\rangle \mid M \text{ se na } w \text{ zastaví}\}$. Je **částečně rozhodnutelný** (stačí $M$ simulovat). **Nerozhodnutelný** – sporem diagonalizací: předpokládáme stroj $H$ rozhodující zastavení, sestrojíme $D$, který pro $\langle M\rangle$ udělá **opak** toho, co $H$ řekne o $M(\langle M\rangle)$; spuštění $D$ na $\langle D\rangle$ → spor.

**6.** Rozhodnutelnost, částečná rozhodnutelnost, nerozhodnutelnost – definice, rozdíl, příklady.
> **Rozhodnutelný** jazyk: TS se pro **každý** vstup zastaví a odpoví správně. **Částečně rozhodnutelný (rekurzivně spočetný)**: TS přijme vstupy z $L$, ale pro vstupy mimo $L$ se může zacyklit. Postova věta: $L$ rozhodnutelný $\iff$ $L$ i jeho doplněk jsou částečně rozhodnutelné. Příklady: rozhodnutelný = prvočíselnost; částečně, ne plně = HALT; ani částečně = doplněk HALT.

**7.** Metoda redukce – definice, princip; diagonalizace – princip.
> **Redukce** $A \le B$: řešení $B$ umožní řešit $A$ (přes vyčíslitelnou převodní funkci). Je-li $A$ nerozhodnutelný a $A \le B$, je i $B$ nerozhodnutelný – standardní technika: redukovat **HALT** na zkoumaný problém. **Diagonalizace** = konstrukce objektu, který se liší od každého prvku spočetného seznamu (jako Cantorův důkaz nespočetnosti) → dokazuje existenci problémů mimo daný výčet.

**8.** Spojení rozhodnutelnosti s Chomského hierarchií.
> **Typ 0** = rekurzivně spočetné = částečně rozhodnutelné (Turingův stroj). **Rozhodnutelné (rekurzivní)** jazyky leží mezi typem 1 (kontextové) a typem 0 – tvoří vlastní třídu, která není přímo v Chomského hierarchii: kontextové $\subset$ rozhodnutelné $\subset$ částečně rozhodnutelné. Existují i jazyky mimo typ 0 (doplněk HALT).

**9.** Existuje problém, co není rozhodnutelný? (ano)
> Ano – např. **problém zastavení**, ekvivalence dvou programů, Postův korespondenční problém. Obecně **Riceova věta**: každá netriviální sémantická vlastnost funkce počítané programem je nerozhodnutelná.

**10.** Je HALT PSPACE-těžký?
> Ano. HALT je nerozhodnutelný, tedy **není v PSPACE**, ale je **PSPACE-těžký**: každý problém z PSPACE je rozhodnutelný, a každý rozhodnutelný problém se dá (many-one) redukovat na HALT – stačí ho vyřešit a podle výsledku zobrazit na pevnou zastavující/nezastavující instanci. HALT je dokonce těžký pro všechny rozhodnutelné třídy.

---

## 11. Složitost

**1.** Složitost algoritmu versus složitost problému.
> **Složitost algoritmu** = počet kroků/paměti konkrétního algoritmu v závislosti na velikosti vstupu (horní mez). **Složitost problému** = složitost nejlepšího možného algoritmu (dolní mez napříč všemi algoritmy). Algoritmus dává horní mez složitosti problému; dolní meze se dokazují obtížně.

**2.** Asymptotická složitost – definice (pomocí konstanty a funkce i limitou).
> Popisuje růst funkce pro velká $n$ (zanedbává konstanty a nižší členy). $O(g)$ horní mez ($f \le c \cdot g$), $\Omega(g)$ dolní mez, $\Theta(g)$ těsný odhad (zároveň $O$ i $\Omega$). Limitně: $f \in O(g)$ pokud $\limsup f/g < \infty$. Příklad: řazení porovnáváním je $\Theta(n\log n)$.

**3.** Složitostní třídy – P, NP, PSPACE, NPSPACE, LOGSPACE, EXPTIME – definice, vztahy mezi nimi.
> **P** – polynomiální čas na deterministickém TS; **NP** – polynomiální čas na nedeterministickém TS (ověření certifikátu v poly čase); **PSPACE/NPSPACE** – polynomiální prostor; **LOGSPACE** – logaritmický prostor; **EXPTIME** – exponenciální čas. Vztahy: $\text{LOGSPACE} \subseteq \text{P} \subseteq \text{NP} \subseteq \text{PSPACE} = \text{NPSPACE} \subseteq \text{EXPTIME}$, ostré $\text{P} \subsetneq \text{EXPTIME}$.

**4.** Co znamená, když problém spadá do NP – simulace nedeterministického TS v polynomiálním čase.
> Existuje nedeterministický TS, který problém vyřeší v poly čase – „uhodne" řešení a ověří ho. Ekvivalentně: existuje polynomiální **verifikátor**, který pro ANO-instanci s **certifikátem** ověří správnost. „Najít je těžké, ověřit snadné." Platí $\text{P} \subseteq \text{NP}$.

**5.** Příklady problémů z jednotlivých tříd.
> **P**: řazení, nejkratší cesta, prvočíselnost (AKS), maximální párování. **NP(-úplné)**: SAT, 3-SAT, barvení grafu, Hamiltonovská kružnice, batoh, klika, vrcholové pokrytí. **PSPACE**: hry (zobecněné šachy/Go), QBF. **EXPTIME**: optimální strategie některých her.

**6.** NP-těžkost, NP-úplnost – definice.
> **NP-těžký** problém $H$: na něj se polynomiálně redukuje **každý** problém z NP ($\forall L \in NP: L \le_p H$) – nemusí být v NP. **NP-úplný**: je zároveň (1) v NP a (2) NP-těžký – nejtěžší problémy v NP. Pokud by jediný NP-úplný byl v P, platilo by $P = NP$.

**7.** Polynomiální redukce – formální definice redukční funkce i problému.
> Funkce $f$ vyčíslitelná v poly čase taková, že $x \in A \iff f(x) \in B$; značíme $A \le_p B$. Pokud $A \le_p B$ a $B \in P$, pak $A \in P$ („$B$ je aspoň tak těžký jako $A$"). Základ definice NP-těžkosti a NP-úplnosti.

**8.** Jak dokázat NP-těžkost problému (redukce z NP-úplného problému).
> Polynomiálně redukovat **nějaký známý NP-úplný problém** (typicky 3-SAT) **na náš** problém: $\text{známý těžký} \le_p \text{náš nový}$. (Pro NP-úplnost navíc ukázat, že náš problém je v NP přes certifikát + verifikátor.)

**9.** Příklady NP-úplných problémů (Subset-sum, 3-SAT).
> SAT (Cook–Levinova věta – první dokázaný NP-úplný), 3-SAT, **Subset-sum**, batoh, barvení grafu, Hamiltonovská kružnice, klika, vrcholové pokrytí. Vzájemně na sebe polynomiálně redukovatelné.

**10.** Savitchova věta – NPSPACE je kvadraticky převoditelné na PSPACE; proč kvadraticky (rekurze šetří paměť).
> **Savitchova věta**: $\text{NSPACE}(f) \subseteq \text{DSPACE}(f^2)$, tedy $\text{NPSPACE} = \text{PSPACE}$. Nedeterministický prostor simulujeme deterministicky s **kvadratickým** nárůstem paměti. Důvod „kvadraticky": rekurzivní procedura $\text{REACH}$ (dosažitelnost konfigurace v $2^k$ krocích přes půlení) **znovupoužívá stejný prostor** pro podvýpočty.

**11.** $P = NP$? (ekvivalent v prostorové složitosti)
> Otázka $P = NP$ je otevřená (obecně se věří $P \neq NP$). **Prostorovým ekvivalentem** je $\text{PSPACE} = \text{NPSPACE}$ – a ta je **dokázána** (Savitchova věta). Tedy u prostorové složitosti determinismus vs nedeterminismus nehraje velkou roli, na rozdíl od otevřeného $P$ vs $NP$.

**12.** Patří regulární jazyky do PSPACE? (ano)
> Ano. Regulární jazyky se rozhodují konečným automatem v **konstantním prostoru** (resp. v $\text{LOGSPACE}$/$P$), a protože $\text{P} \subseteq \text{PSPACE}$, patří i do PSPACE (s velkou rezervou).

**13.** Korektnost a složitost algoritmu – invariant cyklu, důkaz korektnosti řadicího algoritmu (select sort, merge sort).
> **Invariant cyklu** = tvrzení platné před každou iterací; dokazuje se inicializace, zachování, ukončení. U **select sortu** invariant „prvních $i$ prvků je seřazeno a jsou nejmenší". **Merge sort** se dokazuje indukcí (rozděl a panuj). Složitosti: select sort $O(n^2)$, merge sort $O(n\log n)$.

**14.** Složitost quicksortu.
> Průměrně $O(n\log n)$, **nejhorší případ $O(n^2)$** (špatná volba pivotu, např. seřazené pole). In-place, v praxi velmi rychlý díky dobré datové lokalitě.

---

## Matematická logika

> *Není samostatnou otázkou v `Otazky.md`, ale dokazatelnost a rozhodnutelnost logiky navazují na [[#10. Rozhodnutelnost|Rozhodnutelnost]] a [[#11. Složitost|Složitost]].*

**1.** Výroková logika – co to je.
> Logika **výroků** (tvrzení, jež jsou pravdivá/nepravdivá) skládaných **logickými spojkami** ($\neg, \land, \lor, \Rightarrow, \Leftrightarrow$). Neumí kvantifikovat ani popisovat vnitřní strukturu objektů – pracuje jen s atomickými výroky a jejich pravdivostními hodnotami (tabulky pravdivosti).

**2.** Predikátová logika – co to je, příklad (zadat větu, formálně popsat pomocí predikátové logiky prvního stupně).
> **Predikátová logika prvního řádu** rozšiřuje výrokovou o **predikáty** (vlastnosti/vztahy objektů), **proměnné, funkce** a **kvantifikátory** $\forall, \exists$. Příklad: „Každý člověk je smrtelný" → $\forall x\,\big(\text{Člověk}(x) \Rightarrow \text{Smrtelný}(x)\big)$.

**3.** Predikát, interpretace, valuace – definice, konkrétní příklady.
> **Predikát** = funkce vracející pravdivostní hodnotu (např. $\text{Větší}(x,y)$). **Interpretace (struktura)** = volba **univerza** (množiny objektů) a významu predikátů/funkcí/konstant. **Valuace (ohodnocení)** = přiřazení konkrétních objektů z univerza volným proměnným. Formule je pravdivá vzhledem k interpretaci a valuaci.

**4.** Syntax predikátové logiky – co do ní patří.
> **Termy**: proměnné, konstanty, aplikace funkčních symbolů. **Atomické formule**: predikát aplikovaný na termy. **Formule**: atomické + logické spojky + **kvantifikátory** ($\forall x, \exists x$). Syntax určuje, co je dobře utvořená formule (well-formed formula), nezávisle na významu.

**5.** Splnitelnost – definice (existenční kvantifikátor), příklad nesplnitelné formule.
> Formule je **splnitelná**, pokud **existuje** interpretace (a valuace), při níž je pravdivá. **Nesplnitelná** = pravdivá při žádné interpretaci. Příklad nesplnitelné formule (kontradikce): $A \land \neg A$.

**6.** Pravdivost – definice (všeobecný kvantifikátor); vztah splnitelnosti a pravdivosti.
> Formule je **(logicky) pravdivá / tautologie**, pokud je pravdivá při **každé** interpretaci. Vztah: $\varphi$ je pravdivá $\iff \neg\varphi$ je **nesplnitelná**; $\varphi$ je splnitelná $\iff \neg\varphi$ není pravdivá. (Splnitelnost ≈ existence, pravdivost ≈ univerzálnost – jako $\exists$ vs $\forall$.)

**7.** Dokazatelnost – definice, vztah k pravdivosti (korektnost a úplnost důkazových systémů).
> **Dokazatelnost** ($\vdash \varphi$) = formuli lze odvodit v daném **důkazovém systému** (axiomy + odvozovací pravidla). Vztah k pravdivosti ($\models \varphi$): **korektnost (soundness)** – co je dokazatelné, je pravdivé ($\vdash\varphi \Rightarrow \models\varphi$); **úplnost (completeness)** – co je pravdivé, je dokazatelné ($\models\varphi \Rightarrow \vdash\varphi$). Pro predikátovou logiku 1. řádu platí obojí (Gödelova věta o úplnosti).

**8.** Axiomatický systém – znám nějaký? (Łukasiewiczův – 3 axiomy a MP)
> Ano – **Łukasiewiczův** axiomatický systém výrokové logiky: **3 axiomová schémata** (nad spojkami $\Rightarrow, \neg$) + jediné odvozovací pravidlo **modus ponens** (z $\varphi$ a $\varphi\Rightarrow\psi$ odvoď $\psi$). Z nich lze odvodit všechny tautologie.

**9.** Co je to důkaz.
> **Konečná posloupnost formulí**, kde každá je buď axiom, předpoklad, nebo vznikne z předchozích **odvozovacím pravidlem** (např. modus ponens), a poslední formule je dokazované tvrzení.

**10.** Jak to mají stroje s dokazováním – výroková logika se dá dokazovat stroji, predikátová potřebuje omezení na tvar formulí.
> **Výroková logika je rozhodnutelná** – pravdivost lze ověřit strojově (tabulka pravdivosti, SAT solvery; rozhodování je ovšem NP-úplné). **Predikátová logika 1. řádu je jen částečně rozhodnutelná** – dokazatelné formule lze vyjmenovat, ale obecně nelze rozhodnout nepravdivost; proto se **automatické dokazování omezuje na vhodný tvar formulí** (klauzule, Hornovy klauzule).

**11.** Rezoluční metoda.
> Důkazová metoda **sporem** nad formulemi v **konjunktivní normální formě (klauzulemi)**. **Rezoluční pravidlo**: z klauzulí $(A \lor x)$ a $(B \lor \neg x)$ odvodí **rezolventu** $(A \lor B)$. Dokazujeme $\varphi$ tak, že k $\neg\varphi$ rezolucí odvodíme **prázdnou klauzuli** (spor). V predikátové logice se navíc používá **unifikace**. Je základem logického programování (Prolog).

**12.** Reprezentace a vyvozování znalostí.
> Logika slouží k **reprezentaci znalostí** (fakta a pravidla jako formule) a **vyvozování** nových faktů. Příklady: **Hornovy klauzule** a logické programování (Prolog), expertní systémy, ontologie/deskripční logiky. Vyvozování = aplikace inferenčních pravidel (modus ponens, rezoluce) na bázi znalostí.

---
# Programové, výpočetní a informační systémy
---
## 1. Strukturování a řízení běhu programu (Podprogramy a OOP)

**1.** Rozdíl mezi třídou a objektem (objekt je instance třídy).
> **Třída** = předpis/šablona (atributy + metody), **objekt** = konkrétní **instance** třídy v paměti. Z jedné třídy lze vytvořit mnoho objektů s vlastním stavem.

**2.** Kam se ukládá třída (heap/stack/paměť programu); static public atribut – kam se uloží.
> Objekty (instance) se alokují typicky na **haldě**, reference na zásobníku. Samotná **třída** (kód, metadata) je v paměti programu / **metaspace**. **Statický atribut** patří třídě – jediná sdílená kopie v paměti třídy (ne na haldě s objektem).

**3.** Co je static metoda, co když je static atribut.
> **Static metoda** se volá na třídě (`Math.sqrt()`), nemá `this`, nepřistupuje k instančním atributům. **Static atribut** = jediná sdílená kopie pro všechny instance.

**4.** Podprogramy – co to jsou.
> Pojmenované bloky kódu (funkce, procedury, metody) k opakovanému volání. Umožňují znovupoužití, dekompozici, abstrakci. **Funkce** vrací hodnotu, **procedura** jen provede akci. Volání používá **zásobník** (rámec s návratovou adresou a lokálními daty).

**5.** Rozsahy jmen – statický vs dynamický rozsah, příklad jazyka s dynamickým rozsahem (bash).
> **Statický (lexikální) rozsah** – jméno se váže podle **místa v kódu** (C, Java, Python). **Dynamický rozsah** – podle **volajícího kontextu za běhu** (**Bash**, starší Lisp); funkce „vidí" proměnné toho, kdo ji zavolal.

**6.** Příklad kódu – co by bylo vypsáno na stdout u dynamického vs statického rozsahu.
> Mějme globální `x=1` a funkci `f`, která tiskne `x`, a funkci `g`, která lokálně nastaví `x=2` a zavolá `f`. Při **statickém** rozsahu `f` vidí globální `x` → vytiskne **1**. Při **dynamickém** rozsahu `f` vidí `x` z volajícího `g` → vytiskne **2**.

**7.** Předávání hodnot (in/out/inout), jak v Javě změnit předávanou hodnotu.
> **Hodnotou (in)** – kopie, změny se nepromítnou. **Odkazem (inout)** – změny se projeví. **Výstupní (out)** – jen pro vrácení hodnoty. V **Javě** se vše předává **hodnotou**; u objektů se hodnotou předává reference, takže lze měnit **obsah** objektu (ne přepsat samotnou referenci).

**8.** Význam protected, private, public + příklady kdo může přistupovat.
> **private** – jen uvnitř třídy; **protected** – třída + potomci (a balík); **public** – odkudkoli. Atributy bývají private (zapouzdření), přístup přes gettery/settery.

**9.** Výjimky – na co jsou dobré, příklad smysluplné custom výjimky.
> Mechanismus pro ošetření chybových stavů odděleně od hlavní logiky. Výjimka se **vyhodí (throw)** a propaguje zásobníkem, dokud ji někdo **nezachytí (catch)**; nelze ji snadno ignorovat. Smysluplná vlastní: `InsufficientFundsException` při výběru nad rámec zůstatku.

**10.** Event-driven programming.
> Paradigma, kde tok programu řídí **události** (kliknutí, příchod dat, časovač). Program registruje **obslužné rutiny (event handlers/callbacky)**, hlavní smyčka (event loop) čeká na události a volá příslušné handlery. Typické pro GUI a asynchronní/síťové aplikace.

**11.** Co je objekt, zapouzdření, dědičnost, virtuální metody, dynamické vazby.
> **Objekt** = instance třídy. **Zapouzdření** = skrytí vnitřního stavu, přístup jen přes rozhraní. **Dědičnost** = potomek přebírá atributy/metody rodiče (vztah „je"). **Virtuální metoda** = implementace se vybírá podle skutečného typu objektu za běhu. **Dynamická vazba** = navázání volání na implementaci až za běhu (pozdní vazba).

**12.** Polymorfismus – principy, virtuální metody.
> Tentýž kód pracuje s objekty různých typů přes společné rozhraní. Realizováno **virtuálními metodami** a dynamickou vazbou. Příklad: `Zvire z = new Pes(); z.zvuk();` zavolá implementaci z `Pes`.

**13.** Co je třída, co kromě atributů a metod má (events).
> Třída sdružuje **atributy** (stav) a **metody** (chování), dále může mít **konstruktory/destruktory**, **vnořené třídy**, **konstanty**, **statické členy**, **vlastnosti (properties)** a v některých jazycích **události (events)** – mechanismus pro notifikaci posluchačů (delegáti v C#).

**14.** Co se děje při instanciování objektu + popsat konstruktor.
> Při `new`: alokuje se paměť (typicky na haldě), inicializují se atributy, zavolá se **konstruktor** (nastaví počáteční stav, příp. zavolá konstruktor rodiče). Vrátí se reference na objekt.

**15.** Rozdíl mezi overloading a overriding metod.
> **Overloading (přetížení)** – více metod stejného jména, **různé parametry** ve stejné třídě; výběr **staticky** podle typů argumentů. **Overriding (překrytí)** – potomek nahradí metodu rodiče **stejnou signaturou**; výběr **dynamicky** podle typu objektu.

**16.** Abstract class; OOP obecně – výhody a nevýhody.
> **Abstraktní třída** – nelze ji instanciovat, definuje společné rozhraní/část implementace pro potomky. **OOP výhody**: zapouzdření, modularita, znovupoužití (dědičnost), rozšiřitelnost (polymorfismus). **Nevýhody**: režie a složitost, riziko přílišné abstrakce/hluboké hierarchie, horší datová lokalita/výkon.

**17.** Příklad konkrétního kódu s rozsahy jmen (napsat na tabuli).
> Viz otázka 6 – ukázat funkci s lokální a globální proměnnou téhož jména a vysvětlit, kterou definici jméno uvnitř funkce vidí (lexikálně podle umístění v kódu vs dynamicky podle volání).

---

## 2. Principy nízkoúrovňového programování

**1.** Paměťový model programu – co to je, jak se dělí, k čemu slouží segmenty.
> Adresní prostor procesu se dělí na **text (kód)** – strojové instrukce (read-only), **data/BSS** – globální a statické proměnné, **haldu** – dynamická alokace (roste „nahoru"), **zásobník** – lokální proměnné a rámce funkcí (roste „dolů").

**2.** Co se ukládá na haldu a co na zásobník.
> **Zásobník** – lokální proměnné, parametry, návratové adresy; automatická správa (LIFO), rychlý, omezená velikost. **Halda** – dynamicky alokovaná data (`malloc`/`new`), žije do uvolnění, ruční správa, větší.

**3.** Proč je stack menší než halda; přibližná velikost stacku.
> Každé **vlákno má vlastní zásobník** a kontext se přepíná často – velký by plýtval pamětí. Typická velikost **~1–8 MB**. Halda je sdílená v rámci procesu a roste dle potřeby.

**4.** Může se velikost programu měnit za běhu? (OS umí zvětšit prostor)
> Ano – **halda** se za běhu zvětšuje voláním `brk`/`sbrk` nebo `mmap`; OS namapuje další stránky. Zásobník roste automaticky do limitu. Kódový segment je fixní.

**5.** Dynamická alokace – jaké jsou funkce (malloc, free, realloc), co dělají, návratové hodnoty.
> `malloc(size)` alokuje blok, vrací `void*` (nebo `NULL`), obsah neinicializovaný; `calloc` alokuje a vynuluje; `realloc(ptr, size)` změní velikost (může přesunout data a vrátit nový ukazatel); `free(ptr)` uvolní blok.

**6.** Co se stane při double free.
> Dvojí uvolnění téhož bloku → **nedefinované chování**, poškození struktur alokátoru, pád nebo **zneužitelná zranitelnost**.

**7.** malloc – návratový typ (void*), explicitní přetypování, sizeof je operátor (ne funkce).
> `malloc` vrací `void*`; v C++ (a pro čitelnost) se přetypovává na cílový typ: `(int*)malloc(n*sizeof(int))`. `sizeof` je **operátor** vyhodnocovaný při překladu, ne funkce.

**8.** realloc – jak rozšířit pole, když je plné.
> `p = realloc(p, new_size)` – pokud nelze blok rozšířit na místě, alokuje nový větší, **zkopíruje data** a uvolní starý, vrátí nový ukazatel. Pozor: při selhání vrací `NULL`, takže neukládat přímo do `p` (jinak leak).

**9.** Co je ukazatel – definice, operace s ním.
> Proměnná obsahující **adresu** jiné proměnné. Operace: `&x` (adresa proměnné), `*p` (dereference – přístup k hodnotě). Ukazuje na **začátek** paměťového bloku. Umožňuje nepřímý přístup, předávání odkazem, dynamické struktury.

**10.** Co je void pointer, jakou má velikost na různých systémech.
> **`void*`** – generický ukazatel bez typu; **nelze ho dereferencovat ani s ním počítat** (neznámá velikost prvku), nutno přetypovat. Velikost ukazatele je daná architekturou: **4 B na 32bit, 8 B na 64bit**.

**11.** Ukazatelová aritmetika – o kolik se posune při sčítání, zda lze počítat s void pointerem (nelze).
> `p + 1` posune o **velikost jednoho prvku** (`sizeof` typu), ne o 1 bajt – takže `int* + 1` = +4 B. S `void*` aritmetika **nejde** (neznámá velikost prvku).

**12.** Pole a ukazatele – vztah mezi nimi, multipole.
> Jméno pole se ve výrazech chová jako **ukazatel na první prvek** (`arr` ≈ `&arr[0]`); `arr[i]` ≡ `*(arr + i)`. **Vícerozměrné pole** = pole polí, uloženo souvisle (row-major). Pole má pevnou velikost a vlastní paměť, ukazatel je jen adresa.

**13.** Kde přesně ukazuje adresa (na začátek paměťového bloku).
> Ukazatel typicky ukazuje na **začátek (nejnižší adresu)** paměťového bloku/objektu. Dereference čte od této adresy tolik bajtů, kolik určuje typ ukazatele.

**14.** Jak funguje stránkování a jak malloc využívá stránkování.
> Paměť je virtuální, mapovaná na fyzické rámce přes **stránkové tabulky** (po stránkách typicky 4 KiB). `malloc` spravuje haldu a když nemá místo, vyžádá si od OS další **stránky** (přes `brk`/`mmap`).

**15.** Co je string v C – co se uloží na poslední místo (\0).
> Řetězec = **pole znaků zakončené nulovým bajtem `'\0'`**. Terminátor označuje konec (funkce jako `strlen` čtou až k němu). Pro `"ahoj"` (4 znaky) je potřeba pole velikosti **5**. Chybějící terminátor → čtení za hranice.

**16.** Co se stane, když přistoupíme na nealokovanou paměť.
> Pokud stránka není namapovaná → **segmentation fault (SIGSEGV)**; jinak **nedefinované chování** (přepsání cizích dat, tichá chyba).

**17.** Memory leak – co se stane, když nedealokujeme na haldě.
> Alokovaná paměť se **nikdy neuvolní** a ztratí se na ni odkaz; program postupně **spotřebovává paměť** – problém zejména u dlouhoběžících procesů (až vyčerpání paměti).

---

## 3. Architektury

**1.** Číselné soustavy – jaké existují, vztahy mezi nimi, převody (hex-bin-oct-dec) + příklady.
> Poziční soustava: hodnota $= \sum c_i \cdot z^i$, $z$ = základ. Dvojková ($z=2$), desítková ($z=10$), osmičková ($z=8$), šestnáctková ($z=16$). Převod **do desítkové** roznásobením mocnin, **z desítkové** opakovaným dělením základem (zbytky odspodu). **Bin↔Hex** po čtveřicích bitů, **Bin↔Oct** po trojicích. Příklad: $101_2 = 5_{10}$; $1101\,1010_2 = \text{DA}_{16}$.

**2.** Zobrazení celých čísel – přímý, inverzní, doplňkový kód, rozdíly, jak fungují, rozsahy.
> **Bez znaménka**: $0$ až $2^n-1$. **Přímý kód (sign-magnitude)**: nejvyšší bit = znaménko, problém dvě nuly. **Jedničkový (inverzní) doplněk**: záporné = negace bitů, opět dvě nuly. **Dvojkový doplněk** (standard): záporné = negace + 1, jediná nula, rozsah $-2^{n-1}$ až $2^{n-1}-1$.

**3.** Číslo $-4$ ve dvojkovém doplňkovém kódu.
> $4 = 0100_2$; negace $\to 1011$; $+1 \to 1100_2$ (4 bity). V 8 bitech: $4 = 0000\,0100 \to 1111\,1011 + 1 = 1111\,1100_2$.

**4.** Jak zjistit přetečení při sčítání v doplňkovém kódu.
> **Overflow** nastane, když se sčítají dvě čísla **stejného znaménka** a výsledek má **opačné znaménko**. Ekvivalentně: přenos **do** nejvyššího (znaménkového) bitu $\neq$ přenos **z** něj.

**5.** Odčítání čísel na 4bitovém procesoru (přes doplňkový kód).
> $a - b = a + (-b)$, kde $-b$ je dvojkový doplněk. Příklad $5 - 3$: $5 = 0101$, $-3 = 1101$; $0101 + 1101 = 1\,0010$, **přenos zahodíme** → $0010_2 = 2$.

**6.** Reprezentace reálných čísel (IEEE 754), mantisa.
> Číslo ve tvaru $\pm\,\text{mantisa} \times 2^{\text{exponent}}$. Pro 32bit single: **1 bit znaménko, 8 bitů exponent** (s posunem/bias 127), **23 bitů mantisa** (s implicitní jedničkou). Konečná přesnost → zaokrouhlovací chyby (0,1 nelze přesně). Speciální: $\pm 0$, $\pm\infty$, NaN.

**7.** BCD kód; vnější kódy (ASCII, Windows-1250, Unicode).
> **Vnitřní kód** = reprezentace uvnitř počítače; **vnější kód** = pro komunikaci s okolím (ASCII, Windows-1250, Unicode/UTF-8). **BCD (Binary Coded Decimal)** – každá desítková číslice kódována 4 bity zvlášť (např. $25 = 0010\,0101$); snadný převod na text, méně úsporné.

**8.** RISC vs CISC – rozdíly; architektura procesoru.
> **CISC** (x86) – mnoho složitých instrukcí různé délky, instrukce smí pracovat přímo s pamětí, často mikroprogramovaný řadič. **RISC** (ARM, RISC-V, MIPS) – málo jednoduchých instrukcí pevné délky, **load/store** architektura, mnoho registrů, vhodné pro pipeline. **Procesor**: ALU, řadič, registry, PC/IR, sběrnice.

**9.** Kombinační vs sekvenční obvody.
> **Kombinační** – výstup závisí jen na aktuálních vstupech (žádná paměť), z hradel (AND, OR, NOT, XOR); příklady sčítačka, multiplexor. **Sekvenční** – výstup závisí na vstupech i na vnitřním stavu (paměti), základní prvek **klopný obvod**, řízeno hodinovým signálem; příklady registry, čítače.

**10.** Minimalizační metody (K-mapy, Booleova algebra, McCluskey).
> Zjednodušení booleovského výrazu na méně hradel. **Booleova algebra** (de Morgan, distributivita), **Karnaughova mapa** (grafické slučování sousedních jedniček do skupin – mocniny 2), **Quine–McCluskey** (tabulková, algoritmizovatelná pro více proměnných).

**11.** Polosčítačka – tabulka a obvod; RS klopný obvod.
> **Polosčítačka**: součet $S = A \oplus B$ (XOR), přenos $C = A \cdot B$ (AND). Tabulka: $00\to S0\,C0$, $01\to S1\,C0$, $10\to S1\,C0$, $11\to S0\,C1$. **RS klopný obvod**: vstupy $S$ (set → $Q=1$) a $R$ (reset → $Q=0$); $S=R=0$ udrží stav, $S=R=1$ je **zakázaný** stav.

**12.** Von Neumannova architektura – používá se v dnešních počítačích?
> Ano, moderní počítače jsou v jádru **von Neumannovy** (program i data ve společné paměti, jedna sběrnice → von Neumannovo úzké hrdlo). Uvnitř ale mají **oddělené L1 cache** pro instrukce a data (modifikovaná Harvardská architektura) pro vyšší výkon.

---

## 4. Databáze

**1.** Co je relační schéma, relace (z databázového i matematického pohledu).
> **Matematicky**: relace = podmnožina kartézského součinu domén $D_1 \times \dots \times D_n$ (množina $n$-tic). **Databázově**: relace = **tabulka**, řádky = $n$-tice (záznamy), sloupce = atributy. **Relační schéma** = název relace + atributy a jejich domény, např. `Student(id, jméno, ročník)`.

**2.** Klíče – superklíč, kandidátní, primární, cizí klíč.
> **Superklíč** – množina atributů jednoznačně určující $n$-tici (může být nadbytečná). **Kandidátní klíč** – minimální superklíč. **Primární klíč** – zvolený kandidátní klíč. **Cizí klíč** – atribut odkazující na primární klíč jiné relace → referenční integrita.

**3.** Funkční závislosti – co to jsou.
> $X \to Y$ znamená, že hodnota atributů $X$ **jednoznačně určuje** hodnotu $Y$. Příklad: `rodné_číslo → jméno, datum_narození`. Základ pro definici klíčů a normálních forem; Armstrongovy axiomy umožňují odvozovat další závislosti.

**4.** Normální formy – 1NF, 2NF, 3NF (definice, vlastnosti, vztahy mezi nimi), proč se používá normalizace.
> **1NF** – atomické hodnoty. **2NF** – 1NF + žádný neklíčový atribut nezávisí jen na **části** složeného klíče. **3NF** – 2NF + žádná **tranzitivní závislost** neklíčových atributů na klíči. Vnoření $3NF \subset 2NF \subset 1NF$. **Normalizace** odstraňuje redundanci a aktualizační anomálie.

**5.** Boyce-Coddova NF.
> Přísnější varianta 3NF: pro **každou** netriviální závislost $X \to Y$ musí být $X$ **superklíč**. Odstraňuje anomálie při více překrývajících se kandidátních klíčích. $BCNF \subset 3NF$. Někdy nelze dosáhnout BCNF při zachování všech závislostí.

**6.** Relační algebra – selekce, projekce + namapovat na SQL příkazy.
> **Selekce $\sigma$** – vybere řádky splňující podmínku (≈ SQL `WHERE`). **Projekce $\pi$** – vybere sloupce (≈ SQL `SELECT sloupce`). Dále přejmenování $\rho$, spojení $\bowtie$, agregace, množinové operace. Příklad: $\sigma_{ročník=1}(\text{Student})$ ≈ `SELECT * FROM Student WHERE ročník=1`.

**7.** Nakreslit tabulku a ukázat, kde jsou které klíče.
> Např. `Student(id PK, jméno, obor_id FK→Obor.id)`. **Primární klíč** `id` jednoznačně identifikuje řádek; **cizí klíč** `obor_id` odkazuje na primární klíč tabulky `Obor`. Kandidátním klíčem může být i `(jméno, datum_narození)`, pokud je jedinečné.

**8.** ER diagram – nakreslit, popsat vazby.
> Konceptuální model: **entity** (obdélníky), **atributy** (ovály), **vztahy** (kosočtverce) s **kardinalitou** (1:1, 1:N, M:N). M:N vztah se při převodu na schéma realizuje **vazební tabulkou**.

**9.** Rozdíl mezi přirozeným a úplným vnějším spojením (joiny).
> **Přirozené (natural/inner) spojení** spojí $n$-tice se shodnými hodnotami společných atributů; **nespárované řádky vypadnou**. **Úplné vnější spojení (full outer join)** zachová i nespárované řádky z **obou** tabulek a doplní `NULL`. (Levé/pravé zachová z levé/pravé tabulky.)

**10.** Dekompozice relačních schémat.
> Rozdělení schématu na více menších kvůli normalizaci. Musí být **bezeztrátová** (spojením vznikne původní relace) a ideálně **zachovat funkční závislosti**.

**11.** Doména, n-tice, atributy, schéma – popsat, z čeho se skládá relace.
> **Doména** = množina přípustných hodnot atributu. **Atribut** = sloupec (jméno + doména). **$n$-tice** = řádek (záznam). **Schéma** = struktura relace (jméno + atributy a domény). Relace = množina $n$-tic nad daným schématem.

---

## 5. SQL, transakce a zpracování dotazů

**1.** Základní syntaxe SELECT, UPDATE, ALTER TABLE.
> `SELECT sloupce FROM tabulka WHERE podmínka;`, `UPDATE tabulka SET a=1 WHERE id=5;`, `ALTER TABLE tabulka ADD COLUMN c INT;` (mění strukturu – DDL). Příklad: `SELECT jméno FROM Student WHERE ročník=1;`.

**2.** Jednoduchý dotaz – napsat příklad; přidání záznamu do databáze (ne se všemi atributy).
> `INSERT INTO Student (id, jméno) VALUES (1, 'Eva');` – lze i **bez všech atributů**, zbytek dostane `DEFAULT`/`NULL`. Jednoduchý dotaz: `SELECT * FROM Student WHERE ročník = 1;`.

**3.** Integritní omezení – co to jsou, jaké existují, cizí klíč.
> Pravidla zajišťující správnost dat: **PRIMARY KEY** (jednoznačnost + NOT NULL), **FOREIGN KEY** (referenční integrita), **UNIQUE**, **NOT NULL**, **CHECK** (podmínka), **DEFAULT**. DB odmítne operaci, která by omezení porušila.

**4.** Triggery – co to je, k čemu se využívají; uložené procedury.
> **Trigger** – kód **automaticky spuštěný** při události (INSERT/UPDATE/DELETE) na tabulce; použití: auditní log, vynucení pravidel, kaskádové úpravy. **Uložená procedura** – pojmenovaný blok SQL/procedurálního kódu uložený v DB, volaný explicitně.

**5.** Transakce – co to je, ACID vlastnosti, úrovně izolace.
> Posloupnost operací jako **nedělitelný celek**. **ACID**: Atomicita (vše/nic), Konzistence (zachová integritu), Izolace (souběžné transakce se neovlivní), Trvalost (po commitu přežijí pád). **Úrovně izolace** od READ UNCOMMITTED (dirty read) přes READ COMMITTED, REPEATABLE READ po SERIALIZABLE (plná izolace).

**6.** Jak se implementují vlastnosti transakcí (logování, stínové databáze).
> **Logování (write-ahead log)** – před změnou se zapíše do logu, po pádu **redo/undo** → atomicita + trvalost. **Stínové databáze (shadow paging)** – změny do kopií stránek, commit přepne ukazatele. Izolace přes **zamykání / MVCC**.

**7.** Co znamená ROLLBACK.
> Zrušení transakce a vrácení DB do stavu **před jejím začátkem** (opak `COMMIT`). Provede se při chybě nebo na žádost.

**8.** Indexování – co to je, k čemu, řídký vs hustý index, primární/sekundární.
> Pomocná struktura urychlující vyhledávání (za cenu paměti a pomalejších zápisů). **Hustý** – záznam pro každý klíč; **řídký** – jen pro některé (např. začátky bloků). **Primární** – nad seřazeným klíčem (určuje fyzické uspořádání); **sekundární** – nad jiným atributem. Typicky B+ strom nebo hašování.

**9.** Hašování – co to je, proč se nepoužívá MD5/SHA1 pro indexování.
> Hašovací funkce mapuje klíč na přihrádku (bucket) → vyhledání $O(1)$ v průměru, vhodné pro **rovnostní** dotazy (ne rozsahové). **MD5/SHA1** jsou kryptografické haše – zbytečně robustní a **výpočetně drahé**; pro indexy stačí rychlé nekryptografické funkce.

**10.** B+ stromy – jak a proč se používají, jak vypadají, proč jsou vhodné pro databáze.
> Vyvážený strom s vysokým větvením, **data jen v listech**, listy propojené. **Malá výška** → málo přístupů na disk ($O(\log n)$); vnitřní uzly jen směrují → víc klíčů na blok; propojené listy → efektivní **rozsahové dotazy**. Bloky odpovídají velikosti diskové stránky.

**11.** Agregační funkce; CREATE DATABASE, CREATE TABLE.
> **Agregační funkce**: `COUNT, SUM, AVG, MIN, MAX`, často s `GROUP BY` a `HAVING`. Příklad: `SELECT ročník, COUNT(*) FROM Student GROUP BY ročník;`. **DDL**: `CREATE DATABASE skola;`, `CREATE TABLE Student (id INT PRIMARY KEY, jméno VARCHAR(50));`.

---

## 6. Operační systémy

**1.** Architektura OS – z čeho se skládá (jádro, knihovny, démoni, rozhraní).
> **Jádro** – správa HW, procesů, paměti (privilegovaně); **knihovny** – rozhraní aplikací k jádru (libc, wrappery syscallů); **démoni/služby** – procesy na pozadí; **uživatelské rozhraní** – shell, GUI. Po startu jádro spustí **init/systemd** (PID 1).

**2.** Typy jader – monolitické vs mikrojádro, rozdíly; základní režimy procesoru.
> **Monolitické** – vše (ovladače, FS, síť) v jádře, rychlé, chyba shodí systém (Linux). **Mikrojádro** – v jádře jen minimum (IPC, plánování, paměť), služby jako uživatelské procesy, stabilní, ale režie IPC (MINIX, QNX). **Režimy**: kernel mode (privilegovaný) vs user mode (omezený); na x86 ringy 0–3.

**3.** Co je proces, vlákno – rozdíl, sdílí vlákna paměť procesu?
> **Proces** – běžící instance programu s vlastním adresním prostorem, izolovaný. **Vlákno** – „lehký proces" uvnitř procesu, **sdílí adresní prostor** (kód, data, halda, soubory), ale má vlastní zásobník a registry. Ano, vlákna sdílí paměť procesu → snadná komunikace, ale riziko race conditions.

**4.** Virtuální paměť – jak funguje, stránkování, stránkové tabulky, překlad adres (MMU).
> Každý proces vidí vlastní souvislý adresní prostor. Paměť rozdělena na **stránky** a **rámce** (4 KiB); **stránková tabulka** mapuje virtuální stránku → fyzický rámec + příznaky. Překlad zajišťuje **MMU**, urychluje **TLB** (cache překladů). **Page fault** = stránka není v RAM → jádro ji načte.

**5.** Velikost stránky – jak vypočítat.
> Mocnina dvojky (typicky 4 KiB $= 2^{12}$). Počet bitů offsetu $= \log_2(\text{velikost stránky})$, zbytek adresy je číslo stránky. Příklad: 32bit adresa, 4 KiB stránka → 12 bitů offset, 20 bitů číslo stránky ($2^{20}$ stránek).

**6.** Plánování procesů – proč potřebujeme, druhy (FIFO, Round Robin, Shortest Job First).
> Rozhoduje, který proces poběží na CPU (cíl: spravedlnost, propustnost, odezva). **FCFS/FIFO** – fronta, dlouhé úlohy blokují. **SJF** – nejkratší první, optimální čekání, hrozí hladovění. **Round Robin** – časové kvantum, spravedlivé pro interaktivní. Dále prioritní, MLFQ.

**7.** Preemptivní vs kooperativní plánování.
> **Preemptivní** – plánovač může odebrat CPU běžícímu procesu (timer interrupt); lepší odezva, nutná synchronizace. **Kooperativní (nepreemptivní)** – proces běží, dokud se sám nevzdá CPU.

**8.** Deadlock – co to je, kdy nastane, 4 podmínky, jak mu zabránit, jak se detekuje (cyklus v RAG).
> Stav, kdy skupina procesů čeká navzájem na zdroje. **Coffmanovy podmínky** (všechny 4): vzájemné vyloučení, hold and wait, no preemption, kruhové čekání. **Prevence** = porušit některou podmínku (pořadí zámků). **Detekce** = cyklus v grafu alokace zdrojů (RAG) → zabít/restartovat proces.

**9.** Starvation – co to je.
> Proces se neustále odkládá a **nikdy nedostane** potřebný zdroj/CPU (nespravedlivé plánování, priority). Řešení **aging** – postupné zvyšování priority čekajícího. Na rozdíl od deadlocku systém běží, jen konkrétní proces nedostane šanci.

**10.** fork(), join() – jak vzniká proces; copy-on-write.
> **`fork()`** vytvoří téměř identickou kopii procesu (potomka), vrací 0 v potomkovi a PID v rodiči; **`exec()`** nahradí obraz novým programem. Rodič čeká přes `wait()`. **Copy-on-write**: rodič i potomek po fork() sdílejí stránky read-only, kopie vznikne **až při prvním zápisu** → šetří paměť (zvlášť když následuje exec).

> *(Pozn.: standardní POSIX volání pro čekání na potomka je `wait()`/`waitpid()`; `join()` je termín pro vlákna – `pthread_join`.)*

**11.** Kritická sekce; semafory, mutexy, bariéry.
> **Kritická sekce** – úsek kódu se sdíleným zdrojem, kde smí být **jen jedno vlákno** (vzájemné vyloučení). **Mutex** – zámek (jedno vlákno). **Semafor** – čítač povolující N přístupů. **Bariéra** – synchronizační bod, kde vlákna čekají, až dorazí všechna.

**12.** Problém producenta a konzumenta.
> Producent vkládá data do sdíleného **omezeného bufferu**, konzument je odebírá. Producent čeká, je-li buffer plný; konzument, je-li prázdný. Řeší se **semafory** (volná místa, obsazená) + **mutex** na přístup k bufferu.

**13.** Co je program vs proces vs vlákno.
> **Program** – pasivní spustitelný soubor (kód + data) na disku. **Proces** – běžící instance programu s vlastním adresním prostorem a zdroji. **Vlákno** – jednotka výpočtu uvnitř procesu, sdílí jeho adresní prostor; proces má aspoň jedno vlákno.

**14.** Přerušení – jak funguje, typy (SW, vnější).
> Signál přerušující běh CPU a předávající řízení **obslužné rutině (handleru)**. **Hardwarové (vnější)** – od zařízení (klávesnice, časovač, disk), asynchronní. **Softwarové** – vyvolané instrukcí (syscall přes trap). **Výjimky** – chyby za běhu (dělení nulou, page fault). Časovač umožňuje preemptivní plánování.

---

## 7. Souborové systémy

**1.** Blokové zařízení, bloková vrstva, I/O scheduler – po řadě.
> **Blokové zařízení** – čte/zapisuje po **blocích pevné velikosti**, náhodný přístup + buffering (HDD, SSD). **Bloková vrstva** – abstrakce mezi FS a ovladači (fronta I/O, slučování, cache, umožňuje RAID/šifrování/LVM). **I/O scheduler** – řadí požadavky (u HDD minimalizuje pohyb hlavy – elevator algoritmus; u SSD stačí jednoduchý).

**2.** RAID – definice zkratky, RAID 0, RAID 1, RAID 5 – rozdíly.
> **Redundant Array of Independent Disks**. **RAID 0 (striping)** – data přes disky, vyšší výkon a kapacita, **žádná redundance**. **RAID 1 (mirroring)** – data zrcadlena, přežije výpadek disku, poloviční kapacita. **RAID 5** – striping + **distribuovaná parita**, kapacita $n-1$, přežije výpadek **1** disku, pomalejší zápis.

**3.** Proč se u RAID 0 píše na oba disky zároveň (rychlost hlavice HDD).
> U **RAID 0** se data **rozprostřou (stripe)** přes oba disky, takže se zapisují/čtou **paralelně** – každý disk pracuje s jinou částí dat svou hlavou současně → zhruba dvojnásobná propustnost. Nejde o zrcadlení, ale o rozdělení dat.

**4.** Je čtení u RAID 1 rychlejší než u RAID 0? (ano, kvůli hlavicím)
> Pro **čtení** může být RAID 1 srovnatelně/velmi rychlé – stejná data jsou na obou discích, takže lze **rozdělit čtení mezi disky** (nezávislé hlavy obslouží více požadavků současně). Ale **zápis** musí na oba disky (žádné zrychlení), zatímco RAID 0 zrychluje i zápis.

**5.** Jak by vypadal RAID 10, RAID 11 (RAID postavený na RAIDu).
> **RAID 10 (1+0)** – zrcadlené páry (RAID 1) spojené stripingem (RAID 0) → výkon i redundance, poloviční kapacita. „RAID 11" není standardní úroveň – obecně jde o **vnořené (nested) RAID**, kdy se RAID buduje nad jinými RAID svazky.

**6.** Adresářová struktura – jak vypadá, jak vzniká, i-nody.
> Adresáře tvoří **strom** s kořenem `/`. **Adresář je speciální soubor** se seznamem záznamů **(jméno → číslo inode)**, obsahuje `.` (sebe) a `..` (rodič). **Inode** popisuje soubor (kromě jména): typ, práva, vlastník, velikost, časy, počet odkazů, ukazatele na datové bloky.

**7.** Uložení na disku – superblok, inodes, datové bloky, bitmapy.
> Typické rozložení: **boot blok** (zaváděcí kód), **superblok** (metadata celého FS), **bitmapy** (volné inode a datové bloky), **tabulka inode** (metadata souborů), **datové bloky** (obsah souborů a adresářů).

**8.** B+ stromy – jak a proč se používají v souborových systémech.
> Moderní FS (NTFS, btrfs, XFS, ext4 HTree) indexují adresáře a metadata B+ stromy: **malá výška** → málo přístupů na disk i u velkých adresářů ($O(\log n)$ místo lineárního hledání), uzly velikosti bloku, propojené listy → efektivní procházení a rozsahové operace.

**9.** Jaké souborové systémy existují (ext3, ext4, FAT, NTFS).
> Linux: **ext3/ext4** (žurnálovací), XFS, btrfs, ZFS. Windows: **NTFS** (žurnálovací, ACL). Přenosné/USB: **FAT32, exFAT**. macOS: **APFS**. Liší se žurnálováním, velikostí souborů, ACL, snapshoty.

**10.** Fragmentace disku; šifrování disku.
> **Externí fragmentace** – volné místo roztříštěné mezi soubory (nelze uložit souvisle). **Interní** – soubor nezaplní poslední blok (nevyužité místo uvnitř). **Defragmentace** přeskupí data (u SSD zbytečná/škodlivá). **Šifrování disku** (FDE) – transparentní na blokové úrovni (dm-crypt/LUKS, BitLocker, FileVault), symetrická šifra **AES-XTS**, chrání data „at rest".

**11.** Vstup a výstup mapovaný do paměti (memory mapped I/O, mmap).
> Mapování souboru přímo do virtuálního adresního prostoru procesu – přístup pak jako k **poli v paměti** (bez `read`/`write`). Stránky se načítají líně přes page fault, zápisy se zapisují zpět (write-back). Výhody: žádné kopírování kernel↔user buffer, snadné sdílení paměti, vhodné pro velké soubory a načítání knihoven.

> *(Pozn.: pojem „memory-mapped I/O" v kontextu HW znamená i mapování registrů zařízení do adresního prostoru; zde jde o `mmap` souboru, jak míří otázka.)*

**12.** Alokace volného místa.
> Evidence volných bloků **bitmapou** (bit na blok, kompaktní, rychlé hledání souvislých oblastí) nebo **spojovým seznamem** volných bloků. Metody alokace souboru: **souvislá** (rychlá, externí fragmentace), **spojová/FAT** (bez ext. fragmentace, pomalý náhodný přístup), **indexová/inode** (seznam ukazatelů + nepřímé bloky pro velké soubory).

---

## 8. Sítě

**1.** ISO/OSI model – popsat jednotlivé vrstvy, funkce, adresace na každé vrstvě.
> 7 vrstev (odspodu): **fyzická** (bity, signály), **spojová** (rámce, MAC adresy, přístup k médiu), **síťová** (směrování, IP adresy), **transportní** (end-to-end spojení, porty, TCP/UDP), **relační**, **prezentační** (formát/šifrování), **aplikační** (HTTP, DNS). Adresace: MAC na L2, IP na L3, port na L4. Každá vrstva přidává/odebírá hlavičku (zapouzdření).

**2.** Porovnání ISO/OSI s TCP/IP modelem.
> TCP/IP má **4 (5) vrstev**: aplikační (= aplikační+prezentační+relační), transportní (TCP/UDP), síťová/internetová (IP), vrstva síťového rozhraní (= spojová + fyzická). TCP/IP je **praktický** (reálný internet), OSI **referenční/teoretický**.

**3.** Fyzická vrstva – typy kódování (Manchester), výhody/nevýhody; zakódovat 010 v Manchester kódování.
> Přenáší bity jako fyzické signály. **Manchester** kóduje bit **přechodem uprostřed intervalu** (např. konvence: 0 = přechod ↑, 1 = přechod ↓). Výhoda: **samosynchronizace** (hodiny v signálu); nevýhoda: **dvojnásobná šířka pásma**. „010" → ↑ ↓ ↑.
>
> ⚠️ *Konvence se liší: IEEE 802.3 definuje opačně (0 = ↓, 1 = ↑, tj. G.E. Thomas má 0 = ↑). U zkoušky uveď, kterou konvenci používáš.*

**4.** Spojová vrstva – MAC adresy, řízení přístupu k médiu, CSMA/CD, CSMA/CA.
> Přenos rámců mezi sousedními uzly, adresace **MAC** (48bit identifikátor karty). **CSMA/CD** (Ethernet) – naslouchej, vysílej, **detekuj kolize** a opakuj. **CSMA/CA** (Wi-Fi) – **vyhýbání se kolizím** (v rádiu nelze spolehlivě detekovat) + potvrzování.

**5.** Rozdíl mezi switchem a hubem, switchem a bridgem.
> **Hub** (L1) – hloupě opakuje signál na všechny porty (jedna kolizní doména). **Switch** (L2) – **učí se MAC adresy** a posílá rámec jen na cílový port (oddělené kolizní domény). **Bridge** (L2) – spojuje dva segmenty; switch je v podstatě vícePortový bridge.

**6.** Síťová vrstva – směrování, protokoly, IP adresy.
> **Směrování** paketů mezi sítěmi podle **IP adres**, protokol **IP** (best-effort, bez záruky doručení), routery. Podpůrné protokoly: ICMP (diagnostika), ARP (IP→MAC), směrovací protokoly (OSPF, BGP).

**7.** ARP protokol – jak se zjišťují MAC adresy.
> **ARP (Address Resolution Protocol)** zjišťuje **MAC adresu k dané IP** v lokální síti: uzel pošle **broadcast** „kdo má IP X?", vlastník odpoví svou MAC adresou, výsledek se uloží do **ARP cache**.

**8.** Transportní vrstva – TCP vs UDP, rozdíly.
> **TCP** – spojově orientovaný, spolehlivý: handshake, potvrzování, řazení, opakování ztrát, řízení toku a zahlcení (web, e-mail, přenos souborů). **UDP** – nespojový, nespolehlivý: datagramy bez záruky, nízká režie/latence (streaming, hry, DNS, VoIP). Oba používají **porty**.

**9.** Třícestný handshake (SYN, ACK) – podrobně, sekvenční čísla.
> Navázání TCP ve 3 krocích: (1) klient → server **SYN** (seq $x$); (2) server → klient **SYN-ACK** (seq $y$, ack $x{+}1$); (3) klient → server **ACK** (ack $y{+}1$). Obě strany se dohodnou na počátečních sekvenčních číslech. Ukončení čtyřcestně (FIN/ACK).

**10.** Které vrstvy se realizují hardwareově (L1, L2) a které softwareově.
> **Fyzická (L1)** a část **spojové (L2)** se realizují **hardwareově** (síťová karta, PHY, MAC kontrolér). Vyšší vrstvy (síťová L3, transportní L4 a výše) jsou typicky **softwareové** (síťový stack OS, aplikace).

**11.** Přepínání okruhů vs pakety – proč se používají pakety.
> **Přepínání okruhů** vyhradí pevnou cestu na celé spojení (telefon) – garantuje pásmo, ale **plýtvá** při nečinnosti a špatně škáluje. **Přepínání paketů** směruje pakety nezávisle, sdílí linky (**statistické multiplexování**) → efektivnější využití, odolnost vůči výpadkům, za cenu proměnného zpoždění.

**12.** Gateway – jak se propojují sítě na jednotlivých vrstvách.
> **Gateway (brána)** propojuje sítě: na L1 hub/repeater, na L2 switch/bridge, na **L3 router** (mezi IP sítěmi), na vyšších vrstvách aplikační brány (převod protokolů). Multicast doručí jeden paket **skupině** příjemců.

**13.** Topologie sítě (star, bus).
> **Hvězda (star)** – uzly připojené k centrálnímu prvku (switch); výpadek uzlu neohrozí síť, ale centrum je kritické. **Sběrnice (bus)** – sdílené médium, jednoduché, ale kolize a jediný bod selhání. Dále kruh, mesh.

---

## 9. Síťové aplikace a bezpečnost

**1.** Mailové protokoly – SMTP, POP3, IMAP4, jak fungují, kdo s kým komunikuje, porty.
> **SMTP** (25/587) – **odesílání** a přenos pošty mezi servery (push). **POP3** (110/995) – **stažení** pošty na klienta (typicky smaže ze serveru). **IMAP4** (143/993) – přístup k poště **ponechané na serveru**, synchronizace více zařízení. Klient odesílá přes SMTP, čte přes POP3/IMAP.

**2.** Přenos souborů – FTP, rozdíl mezi FTPS a SFTP.
> **FTP** – přenos souborů, **nešifrovaný** (heslo i data v plaintextu), řídicí + datový kanál. **FTPS** – FTP přes **TLS/SSL** (šifrovaná nadstavba FTP). **SFTP** – úplně **jiný protokol přes SSH** (port 22), ne příbuzný FTP.

**3.** DNS – jmenný prostor, hierarchická struktura, TLD, registrátoři.
> **Domain Name System** – překlad doménových jmen na IP. **Hierarchický jmenný prostor**: kořen → **TLD** (.cz, .com) → doména 2. řádu → subdomény. Rekurzivní/iterativní dotazování, výsledky se **cachují** (TTL). **Registrátoři** spravují registrace domén pod TLD. Běží primárně přes UDP (port 53).

**4.** QoS – co to je, co očekáváme od připojení, řízení toku, Token/Leak Bucket, WRED.
> **Quality of Service** – zajištění kvality přenosu (pásmo, zpoždění, jitter, ztrátovost) pro citlivé aplikace (VoIP, video). **Token Bucket** – povolí nárazy do velikosti kbelíku tokenů (řídí průměrnou rychlost). **Leaky Bucket** – vyhladí tok na konstantní rychlost. **WRED** – preventivní zahazování paketů při hrozícím zahlcení.

**5.** Push/Pull model; zabezpečení emailové komunikace – PGP.
> **Push** – odesílatel iniciuje přenos (SMTP doručuje na server). **Pull** – příjemce si data vyžádá (POP3/IMAP stahuje). **PGP** – zabezpečení e-mailu hybridním šifrováním + digitální podpisy; využívá **web of trust** pro důvěru ve veřejné klíče.

**6.** Symetrické vs asymetrické šifrování – rozdíly, příklady (DES, 3DES, AES, RSA).
> **Symetrické** – stejný klíč pro šifrování i dešifrování, **rychlé**, problém s distribucí klíče (AES, DES, 3DES). **Asymetrické** – pár **veřejný/soukromý klíč**, řeší distribuci, ale **pomalé** (RSA).

**7.** Hybridní šifrování.
> Asymetricky se bezpečně přenese **symetrický klíč relace**, samotná data se pak šifrují rychlým symetrickým algoritmem. Spojuje výhody obou – distribuci klíče i rychlost. Používá TLS, PGP.

**8.** Digitální podpisy – jak fungují, je rychlejší podpis nebo šifrování?
> **Podpis** = zašifrování **haše** zprávy soukromým klíčem odesílatele; příjemce ověří veřejným klíčem → autenticita, integrita, nepopiratelnost. Podepisuje se krátký haš (efektivní). U RSA bývá **ověření** veřejným klíčem (malý exponent) **rychlejší** než podepisování soukromým klíčem.

**9.** Zabezpečení na jednotlivých vrstvách (IPSec).
> **Aplikační** – PGP/S-MIME, HTTPS. **Transportní** – **TLS/SSL** (šifruje TCP spojení, hybridní šifrování + certifikáty). **Síťová** – **IPSec** (šifrování/autentizace IP paketů, základ VPN; režimy transport a tunnel). Nižší vrstva = transparentní pro aplikace, vyšší = jemnější kontrola.

**10.** Řízení zahlcení (congestion avoidance).
> Mechanismy bránící přetížení sítě. **TCP** používá okno zahlcení: slow start (exponenciální růst), congestion avoidance (lineární růst, AIMD – additive increase/multiplicative decrease), reakce na ztráty paketů. Aktivní správa front (RED/WRED) zahazuje pakety preventivně.

**11.** Co je VPN a jak funguje; autentizace na aplikační vrstvě.
> **VPN (Virtual Private Network)** – vytvoří **šifrovaný tunel** přes veřejný internet, vzdálený uzel vystupuje jako v lokální síti (důvěrnost + integrita, často IPSec/WireGuard/OpenVPN). **Autentizace na aplikační vrstvě** – např. heslo/token/OAuth v rámci aplikačního protokolu (HTTP Basic, tokeny).

---

## 10. Základy informační bezpečnosti

**1.** Základní bezpečnostní funkce – důvěrnost, integrita, dostupnost, nepopiratelnost původu (vysvětlit pojmy).
> **Důvěrnost** – data vidí jen oprávnění (šifrování, řízení přístupu). **Integrita** – data nejsou neoprávněně změněna (haše, podpisy). **Dostupnost** – služba je dostupná, když je třeba (zálohy, redundance). **Nepopiratelnost původu** – původce nemůže popřít autorství (digitální podpis).

**2.** Symetrické vs asymetrické šifrování – popsat, rozdíly, kdy které použít (na dlouhý soubor).
> **Symetrické (AES)** – rychlé, vhodné na **velký objem / dlouhý soubor**; problém doručit klíč. **Asymetrické (RSA)** – řeší **distribuci klíčů** a podpisy, ale pomalé → jen na malá data / přenos klíče. V praxi **hybridně**: asymetricky se vymění symetrický klíč, jím se šifruje soubor.

**3.** Digitální podpis – jak funguje.
> Zašifrování **haše** zprávy soukromým klíčem odesílatele; ověření veřejným klíčem zaručí **autenticitu, integritu a nepopiratelnost**. Podepisuje se haš (krátký), ne celá zpráva.

**4.** Hašovací funkce – co to je, vlastnosti (slabá a silná bezkolizní), příklady (SHA, MD5).
> Mapuje libovolně dlouhý vstup na výstup pevné délky (otisk). Kryptograficky má být **jednosměrná**, mít **slabou bezkoliznost** (k danému vstupu těžko najít jiný se stejným hašem) a **silnou bezkoliznost** (těžko najít **jakékoli** dva vstupy se stejným hašem). Bezpečné: SHA-2/3; prolomené: MD5, SHA-1.

**5.** Je funkce anything→0 hašovací funkce? (technicky ano, ale velmi špatná)
> Technicky ano (mapuje vstup na výstup pevné délky), ale **kryptograficky bezcenná** – produkuje samé kolize, nesplňuje bezkoliznost ani jednosměrnost v užitečném smyslu.

**6.** RSA – princip, na čem je založen (faktorizace).
> Asymetrická šifra: zvol prvočísla $p, q$; $n = pq$; $\varphi(n) = (p{-}1)(q{-}1)$; zvol $e$ nesoudělné s $\varphi(n)$; $d = e^{-1} \bmod \varphi(n)$. Veřejný klíč $(e, n)$, soukromý $(d, n)$. Šifrování $c = m^e \bmod n$, dešifrování $m = c^d \bmod n$. Bezpečnost stojí na obtížnosti **faktorizace velkého $n$**.

**7.** Kryptografická primitiva – vyjmenovat a popsat.
> Základní stavební bloky: **symetrické šifry** (AES – důvěrnost), **asymetrické šifry** (RSA, ECC – distribuce klíčů, podpisy), **hašovací funkce** (SHA – integrita), **MAC/HMAC** (integrita + autenticita se sdíleným klíčem), **generátory náhodných čísel**, výměna klíčů (Diffie-Hellman). Z primitiv se skládají protokoly (TLS).

**8.** Řízení rizik – kvalitativní/kvantitativní analýza rizik.
> Proces identifikace, hodnocení a ošetření rizik (riziko ≈ hrozba × zranitelnost × dopad). **Kvalitativní** – slovní hodnocení (nízké/střední/vysoké), rychlé, subjektivní. **Kvantitativní** – číselné (např. **ALE** = roční očekávaná ztráta = pravděpodobnost × dopad v penězích). Ošetření: snížit, přenést, přijmout, vyhnout se.

**9.** Audit – co dělá auditor, interní vs externí.
> **Audit** – nezávislé ověření, že bezpečnostní opatření odpovídají politikám/standardům. **Interní** (vlastní zaměstnanci) vs **externí** (nezávislá strana, vyšší důvěryhodnost). Auditor sbírá důkazy, hodnotí a reportuje.

**10.** Common Criteria; hodnocení bezpečnosti – standardy.
> **Common Criteria (ISO 15408)** – mezinárodní standard pro **hodnocení bezpečnosti produktů**, úrovně záruky **EAL1–EAL7**. Další: **ISO/IEC 27001** (systém řízení bezpečnosti informací – ISMS).

---

## 11. Vývoj bezpečných aplikací (Informační bezpečnost)

**1.** Identita a řízení přístupu – co je identita, částečná identita, formy autentizace (hesla, tokeny, biometrika).
> **Identita** = soubor atributů entity; **částečná identita** = podmnožina atributů pro daný kontext. **Formy autentizace** podle faktorů: něco, co **znáš** (heslo, PIN), **máš** (token, karta, mobil), **jsi** (biometrika). **MFA** kombinuje více faktorů.

**2.** Access control list (ACL).
> **ACL (Access Control List)** – seznam u objektu určující, **kdo a jaká práva** k němu má. Opačný pohled je capability list (seznam práv u subjektu).

**3.** Formy řízení přístupu – vyjmenovat a popsat.
> **DAC** (Discretionary) – o právech rozhoduje **vlastník** objektu (unixová práva). **MAC** (Mandatory) – práva vynucuje **systém** podle politiky/klasifikace (SELinux, vojenské). **RBAC** (Role-Based) – práva podle **rolí**. **ABAC** – podle atributů.

**4.** LDAP.
> **Lightweight Directory Access Protocol** – protokol pro přístup k adresářovým službám. **Hierarchická databáze** objektů (uživatelé, skupiny, počítače) ve stromu; slouží k **centrální správě identit a autentizaci** (např. Active Directory).

**5.** Ochrana soukromí – anonymita, pseudoanonymita, nespojitelnost, nepozorovatelnost.
> **Anonymita** – subjekt nelze identifikovat ve skupině. **Pseudonymita** – jednání pod pseudonymem (lze případně propojit s identitou). **Nespojitelnost (unlinkability)** – nelze propojit dvě akce téhož subjektu. **Nepozorovatelnost (unobservability)** – nelze ani zjistit, že akce proběhla.

**6.** Síťové útoky – DoS, DDoS, ARP Spoofing, ICMP flooding, Man-in-the-Middle.
> **DoS/DDoS** – zahlcení služby (z mnoha zdrojů) → nedostupnost. **ARP spoofing / MitM** – útočník se vloží mezi komunikaci. **ICMP flooding** – zahlcení ping pakety. Obrana: šifrování (TLS), autentizace, firewally, IDS/IPS, rate-limiting, statické ARP.

**7.** Jak se útokům předchází.
> Šifrování a autentizace, firewally a segmentace sítě, IDS/IPS, rate-limiting a filtrace (DoS), pravidelné aktualizace, princip nejmenších oprávnění, validace vstupů, bezpečnostní monitoring.

**8.** Bezpečné programování.
> Validace vstupů, ochrana proti injection (SQL, XSS), bezpečná práce s pamětí, princip nejmenších oprávnění, ošetření chyb. Nástroje: **statická analýza (SAST)** – kontrola zdrojového kódu bez spuštění (lintery, SonarQube, Coverity); **dynamická analýza (DAST)** – test za běhu (fuzzing, penetrační testy, sanitizery).

**9.** Použitelná bezpečnost – balancování bezpečnosti a použitelnosti (learnability, memorability, efficiency).
> Bezpečné systémy musí být i **použitelné**, jinak je uživatelé obcházejí. Faktory: **naučitelnost (learnability), zapamatovatelnost (memorability), efektivita (efficiency)**, malá chybovost. Příklad: příliš složitá pravidla na hesla → uživatelé si je píší na papírky (nižší reálná bezpečnost).

**10.** Challenge-response autentizace, replay attack.
> **Challenge-response** – server pošle **náhodnou výzvu (nonce)**, klient odpoví hodnotou závislou na výzvě a tajemství; **heslo neputuje po síti**. **Replay útok** – útočník odposlechne platnou zprávu a **znovu ji přehraje**; brání mu jednorázový nonce / časové razítko (stará odpověď už neplatí).

**11.** Řízení přístupu – autentizace vs autorizace (rozdíl).
> **Autentizace** – ověření „**kdo jsi**" (prokázání identity). **Autorizace** – rozhodnutí „**co smíš**" (jaká práva má ověřená identita). Autentizace předchází autorizaci.
