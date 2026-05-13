# Giulio Bistro — Link in Bio

Link-in-Bio Seite für `bio.giuliobistro.de` — ersetzt Hopp.bio (kostenfrei, eigene Kontrolle).

---

## 🚀 Setup (10 Min)

### 1. Neues GitHub-Repo anlegen

1. Auf [github.com](https://github.com) → **+** oben rechts → **New repository**
2. Name: z.B. `giuliobistro-bio`
3. **Public**
4. **Create repository**

### 2. Dateien hochladen
Die zwei Dateien (`index.html` + `CNAME`) ins neue Repo hochladen.
**Commit changes**.

### 3. GitHub Pages aktivieren
- Settings → Pages
- Source: `main` Branch, `/ (root)`, Save
- Custom domain: `bio.giuliobistro.de` (kommt automatisch aus CNAME-Datei)

### 4. DNS-Record bei domainFACTORY hinzufügen

Bei domainFACTORY → DNS-Einstellungen → **Eintrag hinzufügen**:

| Hostname | Typ | Ziel |
|---|---|---|
| `bio.giuliobistro.de` *(oder nur `bio`)* | **CNAME** | `giuliobistro.github.io.` |

> Punkt am Ende von `giuliobistro.github.io.` wichtig!

### 5. Warten + HTTPS

- 5-30 Min DNS-Propagation abwarten
- Dann in GitHub Pages: **Enforce HTTPS** aktivieren

Fertig!

---

## 🔗 Was anpassen?

Alles steht in `index.html`. Wichtigste Stellen:

**Bio-Text ändern** → Zeile mit `<p class="bio-line">`

**Links bearbeiten** → Suche `<a href="..."` in der `<nav>` Sektion

**Logo-Buchstabe ändern** → `<div class="avatar">G</div>` — statt `G` ein eigenes Bild einfügen:
```html
<img src="logo.jpg" alt="" style="width:100%;height:100%;object-fit:cover;border-radius:50%"/>
```
und Bild ins Repo legen.

**Neuen Link hinzufügen** → einen `<a class="link-btn">...</a>` Block kopieren und Inhalt ändern.

**Reihenfolge ändern** → Buttons im HTML einfach verschieben.

---

## 📱 Wo benutzen?

Den Link `https://bio.giuliobistro.de` setzt du:
- ✅ Instagram Profil Bio
- ✅ TikTok Profil Bio
- ✅ Facebook Page Info
- ✅ Google Business Profile Webseite-Feld

Ein Link → alle wichtigen Aktionen für den Gast.
