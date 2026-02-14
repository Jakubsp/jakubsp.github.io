# Dokumentace vývoje - Pentest Web

Tento projekt byl vytvořen jako portfolio pro Jakuba se zaměřením na pentesting.

## Kroky instalace a nastavení

1.  **Instalace Hugo:**
    *   Proběhla aktualizace balíčků: `sudo apt update`
    *   Instalace Hugo: `sudo apt install -y hugo`
    *   Ověřeno verzí: `hugo version`

2.  **Vytvoření projektu:**
    *   Vytvořen adresář: `/home/jakub/.openclaw/workspace/pentest-web/`
    *   Inicializace Hugo webu: `hugo new site . --force`
    *   Inicializace Git repozitáře: `git init`

3.  **Instalace tématu Blowfish:**
    *   Téma Blowfish bylo přidáno jako Git submodule.
    *   Byla vybrána verze `v2.60.0` pro zajištění kompatibility s instalovanou verzí Hugo (0.131.0).
        `git submodule add https://github.com/nunocoracao/blowfish.git themes/blowfish`
        `cd themes/blowfish && git checkout v2.60.0`

4.  **Konfigurace (hugo.toml):**
    *   Nastaven název webu, jazyk (cs) a téma.
    *   Přidány základní parametry o autorovi a zaměření na TryHackMe Offensive Security path.
    *   Definováno základní menu.

5.  **Ukázkový obsah:**
    *   Vytvořen soubor `content/about.md` s krátkým bio o Jakubovi a jeho cílech v oblasti bezpečnosti.

## Jak spustit lokální server
Pro náhled webu spusťte v tomto adresáři:
```bash
hugo server -D
```
