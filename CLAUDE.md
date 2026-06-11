# Státnicové poznámky – FI MUNI, Programování a vývoj aplikací

## Kontext projektu

Tento projekt slouží k přípravě na státní bakalářskou zkoušku na FI MUNI, obor **Programování a vývoj aplikací**. Cílem je postupně vytvářet výukový materiál pro každou otázku ze souboru `Otazky.md`.

Vstup je téměř vždy **hotová ručně psaná výpiška** (obrázek nebo PDF). Claude funguje jako **přepisovač a korektor** – přepisuje do čistého Markdownu s LaTeXem, opravuje překlepy a zpřesňuje nejasné formulace. Věcný obsah nemění bez souhlasu uživatele.

---

## Struktura projektu

```
/
├── CLAUDE.md               ← tento soubor (instrukce pro Claude)
├── Otazky.md               ← seznam všech státnicových otázek
├── TLDR.md                 ← stručné shrnutí pojmů pro každou otázku
└── teoreticke/
    ├── 01-Linearni-algebra.md   ← referenční styl poznámek
    ├── 02-Matematicka-analyza.md
    └── ...
```

---

## Workflow pro každou otázku

### 1. Uživatel pošle výpisky

Vstup přichází jako **obrázek nebo PDF** s hotovými ručně psanými poznámkami. Claude je přepíše do čistého Markdownu.

### 2. Přepis a korekce (`teoreticke/XX-Nazev.md`)

Claude při přepisu:
- převede veškerý obsah do Markdownu se správnou hierarchií nadpisů
- přepíše všechny matematické výrazy do LaTeXu (`$...$` inline, `$$...$$` blokově)
- opraví překlepy a gramatické chyby
- zpřehlední nejasné nebo rozvleklé formulace – ale **věcný obsah zachová**
- styl a obsažnost přizpůsobí referenčnímu souboru `teoreticke/01-Linearni-algebra.md`
- zkontroluje informace, definice a správnost textu. Zatím neopravuje, zeptá se.

Pokud Claude narazí na místo, kde si **není jistý výkladem, správností nebo čitelností**, nejprve se zeptá – neopravuje věcný obsah sám od sebe.

### 3. Aktualizace TLDR (`TLDR.md`)

- Po dokončení každé otázky Claude přidá do `TLDR.md` stručné shrnutí **všech pojmů z těla otázky**
- Styl: stručné bullet-pointy s tučným názvem pojmu a jednovětným vysvětlením
- Vzor viz existující sekce `## 1. Lineární algebra` v `TLDR.md`

---

## Pravidla pro styl poznámek

Vychází z referenčního souboru `teoreticke/01-Linearni-algebra.md`:

- **Nadpisy** (`#`, `##`, `###`) strukturují témata hierarchicky
- **Tučný text** (`**pojem**`) zvýrazňuje definované pojmy při jejich prvním výskytu
- **Definice** klíčových pojmů jsou uváděny jako citace (`> text`) nebo tučným pojmem s vysvětlením na stejném řádku
- **LaTeX** pro veškeré matematické výrazy – inline `$...$`, blokový `$$...$$`
- **Odrážky** pro vlastnosti, výčty, algoritmy (kroky číslované)
- **Příklady a obrázky** jsou vítány – přidávají konkrétnost
- Jazyk je **český**, terminologie odborná ale přístupná
- **Sekce s otázkami a příklady na konci souboru** (vzor `01`, `02`, `03`): pokud výpiska obsahuje opakovací otázky nebo procvičovací příklady, přepiš je jako text (ne jako obrázek) do sekcí `# Otázky` (konceptuální Q&A) a `# Příklady` (procvičování). Každá otázka je `**N.** zadání` a odpověď je citace `> **Odpověď:** ...` se stručným vysvětlením/postupem.
- **Otázky a příklady vždy přečísluj od 1** – bez ohledu na číslování v originální výpišce (např. otázky 6–10 → 1–5).

---

## Pravidla pro chování Claude

1. **Přepisuj, nepřepisuj obsah.** Věrně přepiš co uživatel napsal – formátování, LaTeX a překlepy jsou volná hra, věcná tvrzení a definice nikoli.
2. **Nejdřív se zeptej, pak oprav.** Pokud je formulace nejasná nebo se zdá chybná, Claude upozorní a zeptá se – neopravuje sám od sebe.
3. **Zachovej strukturu originálu** – pokud uživatel rozdělil téma na sekce, Claude toto členění respektuje a případně jen zpřehlední nadpisy.
4. **Drž se referenčního stylu.** Pokud si nejsi jistý formátem, podívej se na `01-Linearni-algebra.md`.
5. **Po dokončení otázky vždy aktualizuj TLDR.md** – přidej sekci s pojmy z té otázky.
6. **Hotové otázky v `Otazky.md` mají proklik na svůj soubor.** Jakmile poznámka existuje, tučný název otázky se v `Otazky.md` změní na Obsidian wikilink ve tvaru `**[[NN-Nazev-souboru|Zobrazený název]].**`. Na zatím nevytvořené poznámky proklik nedávej (nech obyčejný tučný název). Složky jsou jen `teoreticke/` a `programove/`.

---

## Seznam otázek

### Teoretické základy informatiky a matematika
| # | Název | Soubor | Hotovo |
|---|-------|--------|--------|
| 1 | Lineární algebra | `teoreticke/01-Linearni-algebra.md` | ✅ |
| 2 | Základy matematické analýzy | `teoreticke/02-Matematicka-analyza.md` | ✅ |
| 3 | Popisná statistika | `teoreticke/03-Popisna-statistika.md` | ✅ |
| 4 | Grafy a jejich prohledávání | `teoreticke/04-Grafy-prohledavani.md` | ✅ |
| 5 | Grafové algoritmy | `teoreticke/05-Grafove-algoritmy.md` | ✅ |
| 6 | Stromové datové struktury | `teoreticke/06-Stromove-struktury.md` | ✅ |
| 7 | Návrh algoritmů | `teoreticke/07-Navrh-algoritmu.md` | ✅ |
| 8 | Funkcionální programování | `teoreticke/08-Funkcionalni-programovani.md` | ✅ |
| 9 | Regulární jazyky | `teoreticke/09-Regularni-jazyky.md` | ✅ |
| 10 | Rozhodnutelnost | `teoreticke/10-Rozhodnutelnost.md` | ✅ |
| 11 | Složitost | `teoreticke/11-Slozitost.md` | ✅ |

### Programové, výpočetní a informační systémy
| # | Název | Soubor | Hotovo |
|---|-------|--------|--------|
| 1 | Podprogramy a OOP | `programove/01-OOP.md` | ✅ |
| 2 | Nízkoúrovňové programování | `programove/02-Nizkorovnove-programovani.md` | ✅ |
| 3 | Nízkoúrovňové architektury | `programove/03-Architektury.md` | ✅ |
| 4 | Databáze | `programove/04-Databaze.md` | ✅ |
| 5 | SQL, transakce, dotazy | `programove/05-SQL.md` | ✅ |
| 6 | Operační systémy | `programove/06-Operacni-systemy.md` | ✅ |
| 7 | Souborové systémy | `programove/07-Souborove-systemy.md` | ⬜ |
| 8 | Sítě | `programove/08-Site.md` | ⬜ |
| 9 | Síťové aplikace a bezpečnost | `programove/09-Sitove-aplikace.md` | ✅ |
| 10 | Základy informační bezpečnosti | `programove/10-Informacni-bezpecnost.md` | ✅ |
| 11 | Vývoj bezpečných aplikací | `programove/11-Vyvoj-bezpecnych-aplikaci.md` | ✅ |
| 12 | Paralelní systémy | `programove/12-Paralelni-systemy.md` | ⬜ |
