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
