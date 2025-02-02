# Tagesschau Web Crawler

Ein einfacher Web Crawler, der Nachrichtenartikel von [Tagesschau.de](https://www.tagesschau.de/) extrahiert, speichert und analysiert.

## Funktionen
- 📰 **Extrahiert Nachrichtenartikel** von Tagesschau.de (Titel, Inhalt, Veröffentlichungsdatum und Link).
- 💾 **Speichert die gesammelten Daten** in CSV- und TXT-Dateien.
- 📊 **Analysiert häufige Wörter** aus den Artikeln und Überschriften.

## Verwendung

1. **Crawlen von Artikeln:**
   ```python
   articles = getArt()
   ```

2. **Speichern der Daten:**
   ```python
   saveToCsv(articles)
   saveToTxt(articles, "TagesschauToTxt.txt")
   ```

3. **Häufigste Wörter im Artikeltext analysieren:**
   ```python
   mostCommonWordsFromTxt("TagesschauToTxt.txt", 100)
   ```

4. **Häufigste Wörter in Überschriften analysieren:**
   ```python
   printMostCommonInHeadline(articles, 100)
   ```

## 🛠️ Abhängigkeiten
Das Skript benötigt folgende Python-Bibliotheken:
- `requests`
- `BeautifulSoup`
- `collections.Counter`
- `csv`
- `time`


## ⚠️ Hinweise
- Das Skript pausiert kurz zwischen den Anfragen, um die Server nicht zu überlasten.
- Es verarbeitet nur relevante Artikel und filtert unwichtige Links automatisch aus.

---

📌 **Lizenz**: Dieses Projekt dient nur zu Lernzwecken. Bitte beachte die Nutzungsbedingungen von Tagesschau.de.
