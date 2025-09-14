# Tailwind CSS
Tailwind CSS ist ein modernes CSS-Framework, das auf dem Konzept der Utility-First-Klassen basiert. Anstatt vorgefertigte Komponenten zu liefern, bietet Tailwind eine umfangreiche Sammlung von kleinen, **wiederverwendbaren** CSS-Klassen, die direkt im HTML verwendet werden können.

## Was ist Tailwind?
Tailwind CSS ermöglicht es Designs zu erstellen, indem man viele kleine Utility-Klassen kombiniert. Anstatt eigene CSS-Regeln zu schreiben, nutzt man vordefinierte Klassen wie `bg-blue-500`, `text-center`, `p-4` oder `rounded-lg`.

## Vorteile
- **Schnelle Entwicklung**: Keine eigenen CSS-Dateien nötig, alles über Klassen im HTML
- **Konsistenz**: Einheitliche Spacing-, Farb- und Typografie-Systeme
- **Responsive Design**: Einfache Breakpoint-Klassen (`sm:`, `md:`, `lg:`, `xl:`)
- **Wartbarkeit**: Keine CSS-Konflikte, da alles in einer Datei steht
- **Performance**: Nur verwendete Styles werden in die finale CSS-Datei gepackt

## Nachteile
- **Lernkurve**: Viele Klassen müssen gelernt werden
- **HTML-Verunreinigung**: Viele Klassen im HTML können unübersichtlich werden
- **Framework-Abhängigkeit**: Bindung an Tailwind-spezifische Klassen

## Aufgabenstellung
Erweitere die bestende `index.html`. Wie du siehst, ist eine Liste von Blog-Posts vorhanden. Style diese mit Tailwind. Nutze dabei ausschleisslich Tailwindklassen und keine eigenen CSS-Regeln. Ein Beispiel für Styling mit Tailwind CSS ist shcon vorhanden.

### Vorgehen
1. Studiere die [Tailwind-Dokumentation](https://tailwindcss.com/docs) für verfügbare Klassen.
2. Erweitere die bestehende HTML-Struktur in `index.html`
3. Probiere verschiedene Utility-Klassen aus und kombiniere sie kreativ
4. Teste das responsive Verhalten in verschiedenen Browser-Größen

### Referenz
Die Tailwind-Integration erfolgt über das CDN im `<head>`:
```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

## Nützliche Links
- [Tailwind CSS Dokumentation](https://tailwindcss.com/docs)
- [Utility-First CSS](https://tailwindcss.com/docs/utility-first)
- [Responsive Design](https://tailwindcss.com/docs/responsive-design)
- [Hover, Focus & Other States](https://tailwindcss.com/docs/hover-focus-and-other-states)
- [Spacing](https://tailwindcss.com/docs/padding)
- [Colors](https://tailwindcss.com/docs/customizing-colors)
