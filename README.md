### Test Webprogrammierung 29.05.2024

**Name: Koi Gstrein**
ich werd vielleicht ein paar sachen auf englisch schreiben weil ich es auf deutsch vergessen habe bzw nicht so gut formulieren kann tschuldigung

**Anweisungen:** Beantworten Sie alle Fragen sorgfältig und vollständig. Die maximale Punktzahl für diesen Test beträgt 130 Punkte.

---

#### Teil 1: Planung eines Webprojektes (Relaunch)

**1.1.** Welchen wesentlichen Unterschied gibt es zwischen dem Relaunch einer bestehenden Webseite und der Planung einer neuen Webseite? (5 Punkte)

- Bei einem Relaunch gibt es schon bestehenden Inhalt möglicherweise auch schon bestehenden Code, bei einer neuen Webseite fängt man komplett von vorne an ohne Guidelines

**1.2** Beschreiben Sie die wesentlichen Schritte bei der Planung eines Website-Relaunchs. (10 Punkte)

- Analyse der originellen Website
- Konkurrenzanalyse
- Zielgruppenanalyse
- Inhalte sammeln bzw neu schreiben
- Moodboard, Stylesheet, Screendesign
- Optisches Design
- Technische Ausarbeitung

**1.3** Warum ist es wichtig, eine Bestandsaufnahme der aktuellen Website durchzuführen? Nennen Sie zwei Gründe. (5 Punkte)

- Sieht welche Fehler die vorherige Website hat damit man sie verbessern bzw komplett weglassen kann
- Gibt einem "insight" wie sich die Firma vorher präsentiert hat (kann somit möglicherweise den Geschmack des Kunden sehen usw)

**1.4** Welche Rolle spielt die Zielgruppenanalyse bei einem Website-Relaunch? (5 Punkte)

- Your target audience decides not only the visual identity of your website but also how you create and refine their user experience as they navigate through the website. For example, you would not give an older target audience a website that is very experimental with its design, as they might get confused. You would, however, create that type of website for aspiring media designers as they might be inspired by your work.

---

#### Teil 2: Git und Github

**2.1** Erklären Sie, was Git ist und wofür es verwendet wird. (5 Punkte)
- Git ist ein Repository auf dem man seine Programmierungsdaten speichern kann. Man kann seine Daten mit Git teilen, oder Git als backup verwenden. Man kann auch mithilfe von Git Zusammen an einem Projekt arbeiten da jeder gleichzeitig auf alle Daten Zugriff hat

**2.2** Was ist Github und wie unterscheidet es sich von Git? (5 Punkte)
- Github ist die Platform welche Git hostet

**2.3** Erklären Sie jeden der folgenden Begriffe: (10 Punkte)

* Repository - So wie ein Speicherplatz
* Branch - Zweig, weicht vom main Repository ab, interagiert nicht mit dem main bis man ihn merged
* Commit - Eine Gruppe Daten welche man zusammengesammelt hat zum pushen 
* Merge - Vereint den Zweig mit dem Main
* Pull - Speichert die Änderungen vom Repository ab
* Push - Sendet deine Änderungen in das Repository
* Clone - Downloadet ein Repository
* Remote Repository / Origin
* Fetch - Schaut ob Änderungen im Repository vorhanden sing
* Konflikt - Fehler beim Pushen oder Pullen

---

#### Teil 3: CSS-Variablen nutzen

**3.1** Was sind CSS-Variablen und warum sind sie nützlich? (5 Punkte)
- css variables are simply things like classes, ids, and other such ways in which you decide the identity of the code that you are writing down.

**3.2** Überarbeite den folgenden CSS-Code, indem du redundante Werte identifizierst und entscheidest, welche in CSS-Variablen ausgelagert werden sollten. Achte auf sinnvolle Variablennamen. (10 Punkte)

```css

/* Farben */

.header {
  background-color: #333;
  color: #fff;
}

.button {
  background-color: #007bff;
  color: #fff;
}

.card {
  background-color: #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* Schriftarten */
h1, p {
  font-family: Arial, sans-serif;
}

/* Abstände */

.container {
  margin: 20px;
}

.button {
  border-radius: 5px;
  padding: 10px 20px;
  cursor: pointer;  
}

.header {
  padding: 20px;
}

.card {
  margin-bottom: 20px;
  border-radius: 10px;
  padding: 20px;
}

/* Größen */

.card {
  width: 300px;
}

```

---

#### Teil 4: Komponentenbasierte Elemente für Websites entwickeln

**4.1** Was versteht man unter komponentenbasiertem Webdesign? (5 Punkte)
- Komponenten sind vorgearbeitete gruppen von genau bestimmten Variablen + einem genau bestimmten Aufbau dieser Variablen

**4.2** Nennen Sie zwei Vorteile der Nutzung von komponentenbasierten Elementen. (5 Punkte)
- HTML Aufbau vereinfacht sicht 
- CSS vereinfacht sich auch da das meiste die gleichen ids und classen hat

**4.3** Erstellen Sie ein einfaches Beispiel für eine komponentenbasierte HTML-Struktur (Kartenkomponente mit Bild, Titel, Text). (10 Punkte)

```html
<!-- Beispiel HTML-Struktur für eine Kartenkomponente -->

<div class="container__card">
  <div class="container__cardImage">
    <img src="" alt="alt text" class="cardImage">
  </div>
  <div class="container__cardText">
    <div class="h3">
      <h3 class="containerCardTitle">
        Titel
      </h3>
    </div>
    <div class="paragraph">
      <p class="containerCardParagraph">lorem40</p>
    </div>
  </div>
</div>

```

---

#### Teil 5: Container Queries

**5.1** Was sind Container Queries und wie unterscheiden sie sich von Media Queries? (5 Punkte)
- Container Queries are based on the size of the container, not the size of the viewport 

**5.2** Beschreiben Sie eine Situation, in der Container Queries besonders nützlich sein können. (5 Punkte)
- Wenn sich die Containergröße schneller ändert als die Bildschirmgröße, dann kann man mit Container Queries schauen dass alles noch gut zusammen passt.

**5.3** Erweitern Sie den folgenden **CSS-Code** um eine Container Query, sodass der Innenabstand eines Elements bis zu einer Containerbreite von 400px (width) 20px beträgt. (10 Punkte)

```css

.container {
  width: 500px;
}

.box {
  padding: 40px;
}

/* Container Query */

.container {
  @container(min-width=400px) {
    .box {
      padding: 20px;
    }
  }
}


```

```html
<div class="container">
  <div class="box">
    Dies ist eine Beispiel-Box mit variabler Schriftgröße.
  </div>
</div>
```

---

#### Teil 6: Praktische Aufgabe

Sie erhalten ein bestehendes Webprojekt auf Github und sollen einen Relaunch planen und teilweise umsetzen. Gehen Sie wie folgt vor: (30 Punkte)

0. Erstellen Sie ein Repository "Aufgabe6-Webprog" auf Ihren lokalen Rechner und kopieren Sie den Inhalt aus dem Ordner "Daten" hinein.
1. Erstellen Sie den "initial commit"
2. Erstellen Sie einen neuen Branch mit dem Namen "relaunch".
3. **Durchführen der folgenden Änderungen:**
   - **CSS-Variablen:** Definieren Sie sinnvolle CSS-Variablen und verwenden Sie diese in Ihrer CSS-Datei.
   - **Komponentenbasierte Elemente:** Entwickeln Sie eine einfache, komponentenbasierte HTML-Struktur für eine Kartenkomponente, die einen Titel, ein Bild und einen Text enthält.
   - **Container Queries:** Implementieren Sie eine Container Query, um die Schriftgröße der Kartenkomponente basierend auf der Containergröße anzupassen. Verwenden Sie eine Schriftgröße von 1rem bis zu einer Containerbreite von 540px.
4. **Committen Sie Ihre Änderungen:** Geben Sie nach jedem bedeutenden Schritt einen aussagekräftigen Commit-Namen an und committen Sie Ihre Änderungen.
5. **Merge:** Führen Sie einen Merge des "relaunch"-Branches zurück in den Haupt-Branch ("main") durch.
6. Erstellen Sie auf ihrem Github-Account ein neues öffentliches Repository mit dem Namen "Abgabe-Webprog".
7. Notieren Sie hier die URL zu Ihrem Repo auf Github: https://github.com/bakedbads/daten
8. Pushen Sie Ihr lokales Repository in das neu erstellte Remote-Repository.
9. Speichern Sie zusätzlich alle lokalen Dateien als ZIP-Datei "vorname-nachname.zip" und mailen diese an manuel@startmedia.at