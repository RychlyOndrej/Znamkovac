# 📝 Známkovač / Grader App

[![HTML5](https://img.shields.io/badge/HTML5-Offline-orange?style=flat-square&logo=html5)](https://en.wikipedia.org/wiki/HTML5)
[![No Dependencies](https://img.shields.io/badge/Dependencies-None-success?style=flat-square)](#)
[![Privacy](https://img.shields.io/badge/Privacy-100%25_Local-blue?style=flat-square)](#)

🌍 **[🇨🇿 Česky](#-česky)** | **[🇬🇧 English](#-english)**

---

## 🇨🇿 Česky

**Známkovač** je offline HTML aplikace pro učitele. Umožňuje nastavit hodnotící škálu a analyzovat výsledky (histogram, statistiky). Běží bezpečně a lokálně přímo ve vašem prohlížeči, nepotřebuje připojení k internetu, server ani instalaci.

### ✨ Hlavní funkce

#### 1. Vizuální škála hodnocení
- **Rychlé nastavení**: Výchozí škála odpovídá českému klasifikačnímu stupni 1–5, ale lze ji plně přizpůsobit.
- **Táhla (Drag & Drop)**: Procentuální hranice každého stupně lze jednoduše posunovat vizuálně myší.
- **Zámek poměrů**: Zapnutím funkce „Uzamknout posouvání hranic“ lze s jedním táhlem pohnout všemi ostatními hranicemi přesně v jejich aktuálním poměru.
- **Pořadí řádků**: U každého stupně je vlevo ikona `⠿`, pomocí které lze stupeň přesunout nahoru/dolů (drag & drop), aniž by se rozbila procentuální posloupnost grafu.
- **Výpočet bodů**: Zadáte-li "Maximální počet bodů", aplikace automaticky rozpočítá procentuální hranice do požadovaného bodového zisku (lze nastavit i přesnost na 0–3 desetinná místa).

#### 2. Analýza výsledků (Histogram)
- Pokaždé když v pravém panelu „Zadání studentů“ přidáte studentovi známku, překreslí se graf.
- Graf vizualizuje rozložení známek celého ročníku/třídy a interpoluje jej proložením **křivkou normálního rozdělení**.
- Na grafu je interaktivně vyznačen vzorec pro **medián**.
- Můžete sledovat počty studentů, průměrnou známku a modus.

#### 3. Možnosti exportu
Všechna data lze ukládat pro budoucí navrácení nebo zobrazení:
- **Obyčejná škála (méně dat)**: Tlačítko *Uložit* pod definicemi řádků uloží pouze vaši vlastní vytvořenou tabulku (názvy úseků, barvy a minima).
- **Kompletní výsledky (plná data)**: Tlačítko *Uložit do CSV* uloží nejen škálu, ale i kompletní počty studentů a bodové maximum.
- **Čitelný formát CSV**: Ukládá výstupní data ve snadno pochopitelném CSV a rovnou do něj zapisuje textový rozptyl s bodovým ziskem (např. *54-60b*), abyste si export mohli snadno prohlédnout v Excelu.

> 💡 *Tip: Při kliknutí na export se prohlížeč dotáže, zda si přejete do názvu souboru vložit vlastní příponu (např. jméno třídy).*

### 🚀 Spuštění
1. Otevřete soubor `znamkovac.html` ve svém oblíbeném webovém prohlížeči (Chrome, Firefox, Edge, Safari...).
2. Hotovo.

### 🛡️ Bezpečnost a sdílení (Pro učitele)
Aplikaci můžete snadno sdílet s kolegy (USB klíčenka, e-mail, síťový disk) jednoduše zkopírováním souboru `znamkovac.html`. Nepotřebujete administrátorská práva, aplikace obchází firewally a neposílá data pryč. Všechna citlivá data studentů zůstávají **striktně v lokální paměti prohlížeče**.

---

## 🇬🇧 English

**Grader** is an offline HTML app for teachers to set grading scales and analyze results (histograms, stats). It runs securely and locally right in your browser—no internet connection, server, or installation required.

### ✨ Main Features

#### 1. Visual Grading Scale
- **Quick Setup**: The default scale is set up for standard grading (A–F), but it can be fully customized.
- **Drag & Drop Handles**: Percentage boundaries for each grade can be easily adjusted by dragging them with your mouse.
- **Ratio Lock**: By toggling "Lock boundary movement," moving one slider will proportionally adjust all other boundaries, maintaining their exact current ratios.
- **Row Reordering**: Each grade row has a `⠿` icon on the left. You can drag and drop it to move the grade up or down without breaking the percentage sequence of the chart.
- **Points Calculation**: If you enter "Max Points", the application automatically calculates the specific point thresholds (precision 0–3 decimal places).

#### 2. Results Analysis (Histogram)
- Every time you add a student's grade in the right-hand "Student Input" panel, the chart redraws itself.
- The chart visualizes the grade distribution of the entire class and interpolates it by overlaying a **normal distribution curve**.
- The **median** is interactively highlighted on the chart.
- Track the total number of students, the mean (average), and the mode.

#### 3. Export Options
All data can be saved for future use or viewing:
- **Basic Scale (Fewer Data)**: The *Save* button saves only your custom scale (grade names, colors, minimum percentages).
- **Complete Results (Full Data)**: The *Save to CSV* button saves the scale, complete count of students for each grade, and maximum points.
- **Readable CSV Format**: Saves output data in an easily digestible CSV format. It automatically writes out exact point ranges (e.g., *54-60b*) for clean viewing in Excel without opening the app.

> 💡 *Tip: When you click any export button, the browser will prompt you to optionally add a custom suffix to the generated filename (e.g., the name of the class).*

### 🚀 How to Run
1. Simply open the `grader.html` file in your favorite web browser (Chrome, Firefox, Edge, Safari...).
2. You're done.

### 🛡️ Security & Sharing (For Teachers)
Easily share this application with colleagues via a USB drive, email, or a shared network drive simply by copying the `grader.html` file. You don't need administrator rights to run it, it bypasses firewalls, and it doesn't send data anywhere. All sensitive student data input is kept **strictly in your browser's local memory**.
