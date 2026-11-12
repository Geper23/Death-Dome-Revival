# DEATH DOME REVIVAL — česká dokumentace

[English README](README.md) · [Instalace](docs/INSTALLATION.md) · [Testování](docs/TESTING.md) · [Historie oprav](CHANGELOG.md)

**Neoficiální komunitní projekt pro zachování hry DEATH DOME 2.1.2 a obnovení její funkčnosti na moderních telefonech s Androidem.**

> **Aktuální stav:** V12 — první ověřená hratelná testovací verze. Nejde zatím o záruku funkčnosti celé hry ani všech zařízení.

## O projektu

Cílem DEATH DOME REVIVAL je zachovat původní mobilní hru a její hratelnost. Nejde o remake: soustředíme se na opravy kompatibility původního Android/Unity enginu, zastaralých služeb a dalších překážek spuštění.

## Co už funguje?

| Oblast | Stav |
| --- | --- |
| Spuštění na Androidu 15 | ✅ Ověřeno — Xiaomi Redmi (`tanzanite`) |
| Hlavní menu | ✅ Ověřeno |
| První souboj | ✅ Úspěšně dokončen |
| Spuštění bez nefunkční kontroly serveru | ✅ Ověřeno |
| Další úrovně, inventář, obchod | 🧪 Čeká na delší test |
| Uložený postup po přeinstalaci | 🧪 Neověřeno |
| Čistá instalace sestaveného XAPK | 🧪 Neověřeno |
| Další zařízení a verze Androidu | 🧪 Neověřeno |

**Ověřená sestava:** DEATH DOME 2.1.2 / Revival V12, Android 15. Dosavadní test potvrdil hratelnost na jednom konkrétním telefonu.

## Dosavadní opravy

Experimentální vývoj V1–V12 řešil zejména:
- kompatibilitu starého Android/Unity enginu a nativních knihoven;
- nefunkční kontrolu aktualizací na původních serverech;
- omezení přístupu k identifikátorům telefonu v novém Androidu;
- zastaralé volání ukládání nastavení v reklamní knihovně;
- kompatibilitu podpisu testovacího APK.

Podrobnosti najdeš v [historii oprav](CHANGELOG.md).

## Instalace

Plánovaná distribuce je **XAPK** — jeden soubor obsahující APK a potřebné OBB. Hráč nebude potřebovat kabel USB ani ADB. **Bude ale potřebovat aplikaci schopnou instalovat XAPK včetně OBB dat.**

1. Stáhni autorizované a otestované XAPK z Releases, až bude dostupné.
2. Otevři jej v kompatibilním XAPK instalátoru.
3. Potvrď instalaci podle pokynů Androidu.
4. Ověř spuštění, menu, souboj a ukládání.

**Upozornění:** Čistou instalaci nově sestaveného XAPK zatím nemáme potvrzenou. Funkční V12 neodinstalovávej bez zálohování uloženého postupu. Samotné APK a OBB obvykle neobsahují herní save.

## Problémy a zpětná vazba

Chybu můžeš nahlásit přes [Issues](../../issues). Uveď model telefonu, Android, verzi Revival, způsob instalace a popis problému. Pokud přikládáš logy, nejprve z nich odstraň osobní údaje.

## Právní upozornění

DEATH DOME i původní herní soubory, grafika a značky patří jejich právoplatným vlastníkům. Tento projekt je **nezávislý, neoficiální fanouškovský projekt**, není spojený se společností Glu Mobile ani s vlastníky práv. Originální APK, OBB nebo jiný chráněný obsah není možné zveřejňovat bez potřebných práv či souhlasu.

---

**Projekt spravuje [Geper23](https://github.com/Geper23).**
