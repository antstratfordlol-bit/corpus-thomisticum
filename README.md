# Corpus Thomisticum (S. Thomae de Aquino Opera Omnia in Markdown)

A curated, machine-readable digital corpus of the complete works (*Opera Omnia*) of Saint Thomas Aquinas, formatted in clean UTF-8 Markdown with cross-lingual structural anchors for scholarly research, semantic search, and AI-assisted theology.

```text
corpus-thomisticum/
├── README.md                    # Repository documentation and catalogue
├── _index.md                    # Complete inventory of works, editions, and sigla
├── Summa.*.md                   # Summa Theologiae (1a, 1a2ae, 2a2ae, 3a, Supp) in la, en, es
├── Summa-contra-Gentiles.*.md   # Summa contra Gentiles (Books 1–4) in la, en, es
├── Compendium-theologiae.*.md   # Compendium of Theology in la, en, es
├── QD-*                         # Disputed Questions (De Veritate, De Potentia, De Anima, etc.)
├── Super-*                      # Scriptural commentaries (Gospels and Pauline corpus)
├── Catena-aurea.*.md            # Catena Aurea on the four Gospels in la, en, es
├── De-*                         # Philosophical and theological opuscula
├── Cajetan.*.la.md              # Cardinal Cajetan's commentaries on the Summa Theologiae
└── *.leonine.tsv                # Structural Leonine concordance tables
```

---

## 1. Corpus Overview & Scope

* **Scale**: 159 language editions across 73 distinct works (194 files, ~158 MB).
* **Editions Incorporated**:
  * **Latin (`.la.md`)**: Texts from *Corpus Thomisticum* (Fundación Tomás de Aquino / Enrique Alarcón), the Leonine Commission (*Editio Leonina*), and SCTA (*Scholastic Commentaries and Texts Archive*).
  * **English (`.en.md`)**: Translations by the Fathers of the English Dominican Province (Benziger Brothers, 1947 / CCEL) and Joseph Kenny OP (Dominican House of Studies Priory).
  * **Spanish (`.es.md`)**: Critical translations from the *Biblioteca de Autores Cristianos* (BAC) and the Instituto del Verbo Encarnado (*tomasdeaquino.org*).

---

## 2. Invariant Cross-Lingual Structural Anchors

Every work in this repository is segmented with invariant anchor tags (in HTML anchor format: `{#sigla.reference}`). 

Because the anchors match across languages, a single locator resolves identically across Latin, English, and Spanish texts:
* **Summa Theologiae**: `{#sth.1a.q2.a3}` (Prima Pars, question 2, article 3)
* **Summa contra Gentiles**: `{#scg.1.c13}` (Book 1, chapter 13)
* **De Ente et Essentia**: `{#ente.c1}` (Chapter 1)

This allows instant bilingual or trilingual alignment, parallel reading, and direct citations that adhere to the Santa Croce and Roman academic citation norms.

---

## 3. Contents by Category

### A. The Theological Summae
* **Summa Theologiae**: Complete text in Latin, English, and Spanish across all parts:
  * *Prima Pars* (`1a`)
  * *Prima Secundae* (`1a2ae`)
  * *Secunda Secundae* (`2a2ae`)
  * *Tertia Pars* (`3a`)
  * *Supplementum* (`supp`)
* **Summa contra Gentiles**: Books 1 through 4 in Latin, English, and Spanish.
* **Compendium Theologiae**: In Latin, English, and Spanish.
* **Scriptum super Sententiis**: Commentary on the Sentences of Peter Lombard.

### B. Disputed Questions (*Quaestiones Disputatae*)
* *Quaestiones Disputatae de Veritate* (Truth) in Latin, English, and Spanish.
* *Quaestiones Disputatae de Potentia Dei* (The Power of God) in Latin and English.
* *Quaestio Disputata de Anima* (The Soul) in Latin, English, and Spanish.
* *Quaestio Disputata de Spiritualibus Creaturis* in Latin, English, and Spanish.
* *Quaestiones Disputatae de Virtutibus* (Virtues in General, Charity, Cardinal Virtues) in Latin and English.
* *Quaestio Disputata de Unione Verbi Incarnati* in English.
* *Quaestio Disputata de Malo* in Spanish.
* *Quaestiones Quodlibetales* (Quodlibetal Questions 1–12) in Latin and English.

### C. Major Opuscula
* *De Ente et Essentia* (On Being and Essence) in Latin, English, and Spanish.
* *De Principiis Naturae* (On the Principles of Nature) in Latin, English, and Spanish.
* *De Unitate Intellectus contra Averroistas* in Latin, English, and Spanish.
* *De Substantiis Separatis* (On Separate Substances) in Latin, English, and Spanish.
* *De Aeternitate Mundi* (On the Eternity of the World) in Latin, English, and Spanish.
* *De Regno, ad Regem Cypri* (On Kingship) in Latin, English, and Spanish.
* *De Articulis Fidei et Ecclesiae Sacramentis* in Latin, English, and Spanish.
* *De Rationibus Fidei contra Saracenos, Graecos et Armenos* in Latin and English.
* *De Mixtione Elementorum*, *De Motu Cordis*, *De Sortibus*, and *De Emptione et Venditione*.

### D. Scripture Commentaries
* **Catena Aurea**: Complete commentaries on Matthew, Mark, Luke, and John in Latin, English, and Spanish.
* **Gospel Commentaries**: *Super Evangelium S. Ioannis* and *Super Evangelium S. Matthaei* in Latin and English.
* **Pauline Corpus**: Complete commentaries on Romans, 1 Corinthians, 2 Corinthians, Galatians, Ephesians, Philippians, Colossians, 1 Thessalonians, and Hebrews.
* **Old Testament**: Commentary on the Book of Job (*Expositio super Iob ad litteram*).

### E. Aristotle Commentaries
* *Sententia libri Ethicorum* (Nicomachean Ethics).
* *Sententia super Metaphysicam* (Metaphysics).
* *Sententia super Physicam* (Physics).
* *Sententia super librum De Anima* (On the Soul).
* *Sententia libri Politicorum* (Politics).
* *Expositio libri Posteriorum Analyticorum* and *Peri Hermeneias*.

### F. Mendicant Controversies & Polemical Treatises
* *Contra Impugnantes Dei Cultum et Religionem* in Latin, English, and Spanish.
* *Contra Retrahentes Homines a Religionis Ingressu* in Latin, English, and Spanish.
* *De Perfectione Vitae Spiritualis* in Latin, English, and Spanish.
* *Contra Errores Graecorum* in Latin, English, and Spanish.

### G. Historical Commentaries
* **Cardinal Cajetan (*Tommaso de Vio*)**: Full Latin commentaries on the *Summa Theologiae* (*Prima Pars*, *Prima Secundae*, and *Secunda Secundae*).

---

## 4. How to Use with Agentic Tools & Editors

### Command-Line Search (`ripgrep`)
Because all files are clean UTF-8 text, search across the entire Thomistic corpus is instantaneous:
```bash
# Search for passive potency in the Latin Prima Pars
rg -i "potentia passiva" Summa.1a.la.md

# Search across all disputed questions
rg -i "ratio boni" QD-*
```

### In Claude Code, Antigravity, or Obsidian
Clone the repository locally into your active workspace or knowledge base:
```bash
git clone https://github.com/antstratfordlol-bit/corpus-thomisticum.git
```
You can then pair this corpus directly with the **`study`** skill (for analytical reading by units) and the **`socratic-mentor`** skill (for closed-book oral examination).
