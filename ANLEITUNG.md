# Pottpsycho Website – Anleitung zum Veröffentlichen

Diese Anleitung führt euch durch die Veröffentlichung eurer Website inklusive
Redaktions-Bereich für FAQ & News, eigener Domain und eigenen Mailadressen.

Ihr müsst dafür keinen Code schreiben – nur ein paar kostenlose/günstige
Konten anlegen und Einstellungen klicken.

---

## Schritt 1: GitHub-Konto + Repository

1. Auf https://github.com kostenlos registrieren (falls noch nicht vorhanden).
2. Ein neues Repository erstellen, z. B. `pottpsycho-website` (öffentlich oder privat, beides geht).
3. Den kompletten Inhalt dieses Ordners (`index.html`, `assets/`, `content/`,
   `admin/`) in das Repository hochladen. Am einfachsten geht das über
   "Add file" → "Upload files" auf der GitHub-Website – einfach alle Dateien
   und Ordner reinziehen und "Commit changes" klicken.

## Schritt 2: Netlify-Konto + Deployment

1. Auf https://netlify.com kostenlos registrieren – am einfachsten mit dem
   GitHub-Konto einloggen ("Sign up with GitHub").
2. "Add new site" → "Import an existing project" → GitHub auswählen → euer
   `pottpsycho-website`-Repository auswählen.
3. Build-Einstellungen: einfach leer lassen (kein Build-Befehl nötig, es ist
   eine reine HTML-Seite) und "Deploy" klicken.
4. Nach ein paar Sekunden ist eure Seite unter einer Adresse wie
   `zufälliger-name-123.netlify.app` live erreichbar.

## Schritt 3: Redaktions-Bereich aktivieren (für FAQ & News ohne Code)

1. Im Netlify-Dashboard eurer Seite: "Identity" öffnen → "Enable Identity".
2. Unter Identity → "Settings and usage" → "Registration" auf
   **"Invite only"** stellen (damit sich nicht irgendwer anmelden kann).
3. Unter Identity → "Services" → "Git Gateway" → "Enable Git Gateway".
4. Wieder im Identity-Tab: "Invite users" → eure beiden Mailadressen
   eintragen (Meike & Frank). Ihr bekommt jeweils eine Einladungsmail.
5. Über den Link in der Mail ein Passwort setzen.
6. Ab jetzt erreichbar unter: `eure-domain.de/admin`
   Dort könnt ihr FAQ-Einträge und News direkt bearbeiten – die Website
   aktualisiert sich automatisch, ganz ohne Code.

## Schritt 4: Eigene Domain kaufen & verbinden

1. Domain kaufen, z. B. bei IONOS, Strato oder Namecheap (Vorschlag:
   `pottpsycho.de` oder `pottpsycho-podcast.de`, falls `.de` schon vergeben ist).
2. Im Netlify-Dashboard: "Domain settings" → "Add a domain" → eure gekaufte
   Domain eintragen.
3. Netlify zeigt euch danach die nötigen DNS-Einträge (meist ein "A-Record"
   und/oder "CNAME"). Diese müsst ihr bei eurem Domain-Anbieter (z. B. IONOS)
   im DNS-Bereich eintragen.
4. Das kann bis zu 24 Stunden dauern, bis es überall aktiv ist. Danach ist
   die Seite unter `www.pottpsycho.de` erreichbar (Netlify stellt automatisch
   auch ein kostenloses SSL-Zertifikat für https bereit).

## Schritt 5: Eigene Mailadressen einrichten

Das läuft unabhängig von Netlify, direkt über einen Mail-Anbieter:

- **Günstige Option:** Mailhosting bei eurem Domain-Anbieter (IONOS, Strato)
  – oft schon für wenige Euro im Monat pro Adresse dabei.
- **Empfehlenswerte Option:** Google Workspace (ca. 6 €/Nutzer/Monat) – gibt
  euch Gmail-Oberfläche mit eurer eigenen Domain, z. B. `meike@pottpsycho.de`.
- **Kostenlose Option:** Zoho Mail (kostenloser Tarif für kleine Teams).

Bei jedem Anbieter bekommt ihr ein paar "MX-Einträge", die ihr – genau wie
die Domain-Einträge oben – im DNS-Bereich eures Domain-Anbieters eintragt.

Sobald das läuft, könnt ihr die Mailadressen im Kontakt-Bereich der Website
eintragen (aktuell stehen dort `meike@pottpsycho.de` und
`frank@pottpsycho.de` als Platzhalter).

---

## Was danach?

- **Neue Episoden:** laufen automatisch über den Spotify/YouTube-Player,
  kein Code nötig.
- **FAQ & News:** über `/admin` selbst pflegbar.
- **Größere Änderungen** (neues Design, neue Bereiche, technische
  Erweiterungen): einfach wieder mit mir hier im Chat besprechen – ich passe
  den Code an, ihr müsst nur die neuen Dateien wieder ins GitHub-Repository
  hochladen (Netlify aktualisiert die Seite dann automatisch).
