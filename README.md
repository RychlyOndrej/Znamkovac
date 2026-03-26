(English version below)
# Známkovač (Grading App)

Samostatná, přenositelná HTML aplikace pro učitele na nastavení vizuální hodnotící škály a analýzu výsledků formou histogramu a základní statistiky (medián, průměr, modus). Aplikace běží kompletně lokálně v prohlížeči, nepotřebuje připojení k internetu, server ani instalaci. Vše probíhá bezpečně u vás na počítači.

## Hlavní funkce

### 1. Vizuální škála hodnocení
- **Rychlé nastavení**: Výchozí škála odpovídá českému klasifikačnímu stupni 1–5, ale lze ji plně přizpůsobit.
- **Táhla (Drag & Drop)**: Procentuální hranice každého stupně lze jednoduše posunovat vizuálně myší.
- **Zámek poměrů**: Zapnutím funkce „Uzamknout posouvání hranic“ lze s jedním táhlem pohnout všemi ostatními hranicemi přesně v jejich aktuálním poměru.
- **Pořadí řádků**: U každého stupně je vlevo ikona `⠿`, pomocí které lze stupeň přesunout nahoru/dolů (drag & drop), aniž by se rozbila procentuální posloupnost grafu.
- **Výpočet bodů**: Zadáte-li "Maximální počet bodů", aplikace automaticky rozpočítá procentuální hranice do požadovaného bodového zisku (lze nastavit i přesnost na 0-3 desetinná místa).

### 2. Analýza výsledků (Histogram)
- Pokaždé když v pravém panelu „Zadání studentů“ přidáte studentovi známku, překreslí se graf.
- Graf vizualizuje rozložení známek celého ročníku/třídy a interpoluje jej proložením **křivkou normálního rozdělení**.
- Na grafu je interaktivně vyznačen vzorec pro **medián**.
- Můžete sledovat počty studentů, průměrnou známku a modus.

### 3. Možnosti exportu
Všechna data lze ukládat pro budoucí navrácení, nebo zobrazení:

- **Obyčejná škála (méně dat)**: Spodní tlačítko *Uložit* pod definicemi řádků uloží pouze vaši vlastní vytvořenou tabulku (názvy úseků, barvy a jejich minimální procenta).
- **Kompletní výsledky (plná data)**: Tlačítko *Uložit do CSV* uloží nejen škálu, ale i kompletní počty studentů v každé známce a bodové maximum.
- **Čitelný formát CSV**: Systém ukládá výstupní data ve snadno pochopitelném CSV a rovnou do něj zapisuje maximální procentuální limit pro daný řádek i přesný textový rozptyl s bodovým ziskem (např. *54-60b*) tak, abyste si exportní soubor mohli snadno prohlédnout v Excelu bez spuštění aplikace.

*Tip: Při kliknutí na jakýkoli export se vás prohlížeč dotáže, zdali si nepřejete do názvu generovaného souboru vložit vlastní příponu (např. jméno třídy).*

## Spuštění

1. Otevřete jednoduše soubor `znamkovac.html` ve svém oblíbeném webovém prohlížeči (Chrome, Firefox, Edge, Safari...).
2. Hotovo.

## Učitelům
Aplikaci můžete snadno sdílet s kolegy skrze USB klíčenku, e-mail či síťový disk jednoduše nakopírováním `znamkovac.html` – nepotřebujete administrátorská práva pro její chod, obchází firewally a neposílá data pryč. Všechna vámi zapsaná citlivá data studentů se drží striktně v lokální paměti prohlížeče.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


**Grader (Grading App)**
A standalone, portable HTML application for teachers to set up a visual grading scale and analyze results via a histogram and basic statistics (median, mean, mode). The application runs completely locally in the browser—it does not need an internet connection, server, or installation. Everything happens securely on your own computer.

**Main Features**
1. Visual Grading Scale
Quick Setup: The default scale is set up for standard grading (A–F), but it can be fully customized.

Drag & Drop Handles: The percentage boundaries for each grade can be easily adjusted by dragging them with your mouse.

Ratio Lock: By toggling "Lock boundary movement," moving one slider will proportionally adjust all other boundaries, maintaining their exact current ratios.

Row Reordering: Each grade row has a ⠿ icon on the left. You can drag and drop it to move the grade up or down without breaking the percentage sequence of the chart.

Points Calculation: If you enter the "Max Points", the application automatically calculates the specific point thresholds for your percentage boundaries (you can also set the precision to 0–3 decimal places).

2. Results Analysis (Histogram)
Every time you add a student's grade in the right-hand "Student Input" panel, the chart redraws itself.

The chart visualizes the grade distribution of the entire class and interpolates it by overlaying a normal distribution curve.

The median is interactively highlighted on the chart.

You can track the total number of students, the mean (average), and the mode.

3. Export Options
All data can be saved for future use or viewing:

Basic Scale (Fewer Data): The Save button under the grade definitions saves only your custom scale (grade names, colors, and minimum percentages).

Complete Results (Full Data): The Save to CSV button saves both the scale and the complete count of students for each grade, alongside the maximum points.

Readable CSV Format: The system saves the output data in an easily digestible CSV format. It automatically writes out the exact point ranges (e.g., 54-60b), meaning you can cleanly view the export in Excel without even opening the app.

Tip: When you click any export button, the browser will prompt you to optionally add a custom suffix to the generated filename (e.g., the name of the class).

**How to Run**
Simply open the grader.html file in your favorite web browser (Chrome, Firefox, Edge, Safari...).

You're done.

For Teachers
You can easily share this application with colleagues via a USB drive, email, or a shared network drive simply by copying the grader.html file. You don't need administrator rights to run it, it bypasses firewalls, and it doesn't send data anywhere. All the sensitive student data you input is kept strictly in your browser's local memory.
