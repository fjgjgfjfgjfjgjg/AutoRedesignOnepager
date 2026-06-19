# AutoRedesign — Landing Page

Statische Landingpage für **AutoRedesign** (by homepageupgrade.de).
Eine einzige, selbstständige `index.html` — keine Build-Schritte, keine Abhängigkeiten.
Läuft auf jedem Static-Host (Vercel, Netlify, GitHub Pages …).

## Inhalt
```
.
├── index.html      ← die komplette Seite (Bilder & Code eingebettet)
├── vercel.json     ← optionale Vercel-Konfiguration
└── README.md
```

## Lokal ansehen
`index.html` einfach im Browser öffnen (Doppelklick) — fertig.

---

## 1) Auf GitHub einrichten

**Variante A – über die Weboberfläche (am einfachsten):**
1. Auf <https://github.com/new> ein neues Repository anlegen, z. B. `autoredesign-landing`.
2. „uploading an existing file" wählen und **alle Dateien aus diesem Ordner** hochladen (`index.html`, `vercel.json`, `README.md`).
3. „Commit changes".

**Variante B – über die Kommandozeile:**
```bash
cd dieser-ordner
git init
git add .
git commit -m "AutoRedesign Landing Page"
git branch -M main
git remote add origin https://github.com/DEIN-NAME/autoredesign-landing.git
git push -u origin main
```

---

## 2) Über Vercel deployen

1. Auf <https://vercel.com> mit dem GitHub-Account einloggen.
2. **„Add New… → Project"** klicken.
3. Das Repository `autoredesign-landing` auswählen → **Import**.
4. Bei *Framework Preset* **„Other"** lassen (es ist eine statische Seite, kein Build nötig).
   - Build Command: *(leer lassen)*
   - Output Directory: *(leer lassen)*
5. **Deploy** klicken.

Nach ~20 Sekunden ist die Seite live unter `https://autoredesign-landing.vercel.app`
(bzw. dem von dir gewählten Projektnamen).

### Eigene Domain verbinden
Vercel-Projekt → **Settings → Domains** → Domain eintragen und den angezeigten
DNS-Eintrag bei deinem Domain-Anbieter setzen.

---

## Änderungen / Updates
Diese `index.html` ist die exportierte Endfassung. Inhaltliche Änderungen am besten
in der Quelldatei (`AutoRedesign.dc.html`) vornehmen, neu exportieren und die
`index.html` im Repo ersetzen — Vercel deployt bei jedem `git push` automatisch neu.
