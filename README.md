
<div align="center">
  <img src="ollama-nextjs-ui.gif">
</div>

<h1 align="center">
  Voll ausgestattete & schöne Weboberfläche für Ollama LLMs
</h1>

<div align="center">
  
![GitHub Repo stars](https://img.shields.io/github/stars/jakobhoeg/nextjs-ollama-llm-ui)
  
</div>

Starte mit großen Sprachmodellen **schnell**, **lokal** und sogar **offline**.
Dieses Projekt zielt darauf ab, der einfachste Weg zu sein, um mit LLMs zu beginnen. Keine lästige und zeitaufwendige Einrichtung erforderlich!

# Funktionen ✨

- **Schöne & intuitive Benutzeroberfläche:** Inspiriert von ChatGPT, um eine ähnliche Benutzererfahrung zu bieten.
- **Vollständig lokal:** Speichert Chats in LocalStorage für Komfort. Keine Datenbank erforderlich.
- **Vollständig responsive:** Nutze dein Handy, um mit der gleichen Leichtigkeit wie am Desktop zu chatten.
- **Einfache Einrichtung:** Keine lästige und zeitaufwendige Einrichtung. Einfach das Repo klonen und loslegen!
- **Code-Syntax-Hervorhebung:** Nachrichten mit Code werden für besseren Zugriff hervorgehoben.
- **Einfaches Kopieren von Codeblöcken:** Hervorgehobenen Code mit einem Klick kopieren.
- **Modelle herunterladen und löschen:** Modelle direkt über die Oberfläche herunterladen und löschen.
- **Zwischen Modellen wechseln:** Schneller Wechsel zwischen Modellen mit einem Klick.
- **Chatverlauf:** Chats werden gespeichert und sind leicht zugänglich.
- **Heller & Dunkler Modus:** Wechsel zwischen hellem und dunklem Modus.

# Vorschau

https://github.com/jakobhoeg/nextjs-ollama-llm-ui/assets/114422072/08eaed4f-9deb-4e1b-b87a-ba17d81b9a02

# Voraussetzungen ⚙️

Um die Weboberfläche zu nutzen, müssen diese Voraussetzungen erfüllt sein:

1. Lade [Ollama](https://ollama.com/download) herunter und lasse es laufen. Alternativ kannst du es in einem Docker-Container betreiben. Sieh dir die [Dokumentation](https://github.com/ollama/ollama) für Anweisungen an.
2. Node.js (18+) und npm sind erforderlich. [Herunterladen](https://nodejs.org/en/download)

# Eigene Bereitstellung auf Vercel oder Netlify mit einem Klick ✨

[![Mit Vercel bereitstellen](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fjakobhoeg%2Fnextjs-ollama-llm-ui&env=NEXT_PUBLIC_OLLAMA_URL&envDescription=Your%20Ollama%20URL) [![Mit Netlify bereitstellen](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/jakobhoeg/nextjs-ollama-llm-ui)

Du musst deine [OLLAMA_ORIGINS](https://github.com/ollama/ollama/blob/main/docs/faq.md) Umgebungsvariable auf dem Gerät setzen, auf dem Ollama läuft:

```
OLLAMA_ORIGINS="https://your-app.vercel.app/"
```

# Installation 📖

[![Paketstatus](https://repology.org/badge/vertical-allrepos/nextjs-ollama-llm-ui.svg?columns=3)](https://repology.org/project/nextjs-ollama-llm-ui/versions)

Verwende ein vorgefertigtes Paket von einem der unterstützten Paketmanager, um eine lokale Umgebung der Weboberfläche zu betreiben.
Alternativ kannst du von der Quelle installieren, indem du die untenstehenden Anweisungen befolgst.

> [!HINWEIS]  
> Wenn dein Frontend auf einer anderen Adresse als `http://localhost` oder `http://127.0.0.1` läuft, musst du die OLLAMA_ORIGINS auf die URL deines Frontends einstellen.
>
> Dies ist auch in der [Dokumentation](https://github.com/ollama/ollama/blob/main/docs/faq.md#how-do-i-configure-ollama-server) beschrieben:
> 
> `Ollama erlaubt standardmäßig Cross-Origin-Anfragen von 127.0.0.1 und 0.0.0.0. Zusätzliche Ursprünge können mit OLLAMA_ORIGINS konfiguriert werden.`

## Installation von der Quelle

**1. Klone das Repository in ein Verzeichnis auf deinem PC über die Kommandozeile:**

```
git clone https://github.com/jakobhoeg/nextjs-ollama-llm-ui
```

**2. Öffne den Ordner:**

```
cd nextjs-ollama-llm-ui
```

**3. Benenne die `.example.env` Datei in `.env` um:**

```
mv .example.env .env
```

**4. Wenn deine Ollama-Instanz NICHT auf der Standard-IP-Adresse und dem Standard-Port läuft, ändere die Variable in der .env-Datei entsprechend:**

```
NEXT_PUBLIC_OLLAMA_URL="http://localhost:11434"
```

**5. Installiere die Abhängigkeiten:**

```
npm install
```

**6. Starte den Entwicklungsserver:**

```
npm run dev
```

**7. Gehe zu [localhost:3000](http://localhost:3000) und beginne, mit deinem Lieblingsmodell zu chatten!**

# Zukünftige Funktionen

Dies ist eine To-Do-Liste der kommenden Funktionen.
- ✅ Sprachunterstützung
- ✅ Code-Syntax-Hervorhebung
- ⬜️ Möglichkeit, ein Bild in den Prompt zu senden, um visuelle Sprachmodelle zu nutzen.
- ⬜️ Möglichkeit, Antworten zu regenerieren.
- ⬜️ Chats importieren und exportieren.

# Tech-Stack

[NextJS](https://nextjs.org/) - React-Framework für das Web

[TailwindCSS](https://tailwindcss.com/) - Utility-First CSS-Framework

[shadcn-ui](https://ui.shadcn.com/) - UI-Komponenten, gebaut mit Radix UI und Tailwind CSS

[shadcn-chat](https://github.com/jakobhoeg/shadcn-chat) - Chat-Komponenten für NextJS/React-Projekte

[Framer Motion](https://www.framer.com/motion/) - Motion/Animationsbibliothek für React

[Lucide Icons](https://lucide.dev/) - Icon-Bibliothek

# Nützliche Links

[Medium Artikel](https://medium.com/@bartek.lewicz/launch-your-own-chatgpt-clone-for-free-on-colab-shareable-and-online-in-less-than-10-minutes-da19e44be5eb) - Wie du deinen eigenen ChatGPT-Klon kostenlos auf Google Colab startest. Von Bartek Lewicz.

[Lobehub-Erwähnung](https://lobehub.com/blog/5-ollama-web-ui-recommendation#5-next-js-ollama-llm-ui) - Fünf ausgezeichnete kostenlose Ollama WebUI-Client-Empfehlungen
```
