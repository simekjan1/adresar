# Adresář

Jednoduchá offline aplikace pro správu kontaktů s důrazem na přístupnost, soukromí a rychlé ovládání.

## O projektu

Adresář vznikl původně jako moje soukromá aplikace pro správu kontaktů.

V současnosti není zamýšlen jako veřejná služba ani jako hotový produkt pro ostatní uživatele. Zdrojový kód je přesto umístěn ve veřejném GitHub repozitáři, protože aplikaci používám prostřednictvím GitHub Pages a pro tento způsob nasazení potřebuji veřejný repozitář.

Veřejný je pouze zdrojový kód aplikace. Moje kontakty ani jiná osobní data nejsou součástí repozitáře.

Do budoucna nevylučuji, že projekt zveřejním i jako aplikaci určenou ostatním uživatelům. Zatím jde především o nástroj vytvořený pro moje vlastní použití.

## Hlavní vlastnosti

- lokální ukládání kontaktů pomocí IndexedDB,
- žádný cloud ani synchronizace,
- žádná analytika ani telemetrie,
- žádné externí knihovny nebo síťové služby,
- skupiny kontaktů,
- globální vyhledávání,
- více telefonních čísel a e-mailů u jednoho kontaktu,
- volání, SMS a e-mail pomocí systémových aplikací,
- Koš bez automatického mazání,
- kompletní záloha a obnova pomocí JSON,
- import a export kontaktů ve formátu VCF/vCard,
- ovládání z klávesnice,
- přístupnost pro odečítače obrazovky včetně Android TalkBacku,
- responzivní tmavé rozhraní.

## Soukromí

Aplikace neposílá kontakty na server.

Data jsou ukládána lokálně v IndexedDB konkrétního prohlížeče. GitHub Pages slouží pouze k distribuci samotné aplikace.

Zdrojový kód neobsahuje databázi kontaktů.

Pro bezpečné uchování dat je možné vytvořit úplnou JSON zálohu. Uživatel je odpovědný za bezpečné uložení exportovaných JSON a VCF souborů.

> Důležité: Vymazání dat webu nebo úložiště prohlížeče může odstranit lokálně uloženou databázi. Pravidelné JSON zálohy jsou proto doporučené.

## Přístupnost

Přístupnost byla jedním z hlavních požadavků při návrhu aplikace.

Rozhraní je navrženo pro:

- Android TalkBack,
- ovládání pomocí klávesnice,
- viditelný focus,
- logické pořadí ovládacích prvků,
- sémantické HTML,
- vysoký kontrast a jednoduché rozhraní.

Aplikace byla prakticky testována s TalkBackem na Androidu i pomocí klávesnice na počítači.

## Technologie

Celá aplikace je obsažena v jediném souboru `adresar.html`.

Používá pouze:

- HTML,
- CSS,
- JavaScript,
- IndexedDB.

Nejsou potřeba žádné externí závislosti ani instalace.

## Stav projektu

**Aktuální verze: 1.0**

Verze 1.0 je funkční a používám ji v běžném provozu.

Další vývoj bude vycházet především ze zkušeností při skutečném používání. Případná verze 1.1 proto vznikne až podle toho, které změny a nové funkce se ukážou jako skutečně užitečné.

## Upozornění

Projekt je v současnosti vytvářen především pro moje vlastní použití. Veřejná dostupnost zdrojového kódu neznamená, že garantuji podporu, kompatibilitu nebo další vývoj.