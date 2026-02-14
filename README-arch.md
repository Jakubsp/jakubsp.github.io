# Pentest Portfolio Architecture - Jakub

Tento dokument definuje architekturu a strukturu webového portfolia pro Jakuba, zaměřeného na **Offensive Security** (TryHackMe, OSCP path).

## 1. Technologický Stack (Návrh)

Doporučená volba: **Hugo**
- **Proč?** Neuvěřitelná rychlost, statické HTML (bezpečné!), skvělá podpora pro Markdown (vhodné pro writeupy) a bohatá komunita v infosec sféře.
- **Hosting:** GitHub Pages (zdarma, nativní integrace).
- **Doména:** `jakub.github.io` (nebo vlastní `.cz`/`.com` nasměrovaná na GitHub).

### Doporučená Témata:
1.  **Blowfish** (Moderní, čisté, skvělé pro dokumentaci a projekty).
2.  **Terminal** (Retro "hacker" look, velmi oblíbené u pentesterů).
3.  **PaperMod** (Minimalistické, rychlé, profesionální).

---

## 2. Struktura Webu (Content Architecture)

```text
/content
├── _index.md                # Home page (Bio, Quick Links, Skills)
├── about.md                 # Podrobné CV, certifikace, kontakty
├── writeups/                # Návody a řešení strojů (THM/HTB)
│   ├── tryhackme/           # Konkrétně sekce pro Offensive Security path
│   └── htb/
├── projects/                # Vlastní skripty, tooly na GitHubu
└── blog/                    # Myšlenky, poznámky z výzkumu, CVE analýzy
```

---

## 3. Klíčové Sekce pro Zaměstnavatele

1.  **Skills Matrix:** Jasný přehled (Recon, Web Apps, Network, PrivEsc, AD).
2.  **TryHackMe Badge/Profile:** Integrace THM API nebo widgetu pro zobrazení progresu.
3.  **Github Feed:** Ukázka kódu (Python/Bash skripty pro automatizaci).
4.  **Writeups:** Kvalita nad kvantitou. Ukázat *způsob uvažování* (methodology), ne jen flagy.

---

## 4. Deployment Pipeline

1.  Repozitář na GitHubu (`portfolio`).
2.  **GitHub Actions:** Automatický build a deploy při každém `git push` do větve `main`.
3.  Bezpečné uložení případných tajných klíčů v GitHub Secrets (pokud budou potřeba např. pro API).

---

## 5. První kroky (Roadmap)

1.  [ ] Inicializace Hugo repozitáře.
2.  [ ] Výběr a instalace tématu (Git Submodule).
3.  [ ] Nastavení `hugo.toml` (základní metadata).
4.  [ ] Vytvoření první stránky `about.md` s certifikacemi.
5.  [ ] Nastavení GitHub Actions workflow.

---
*Vytvořeno automaticky pro Jakuba (Pentest Web Arch).*
