# Atar.Bot InSites — CBSA Heritage Assessment AI

## About

**Atar.Bot InSites** is an AI-powered assistant designed to guide heritage professionals through Context-Based Significance Assessment (CBSA) — a holistic methodology for evaluating cultural heritage sites.

This repository contains the core AI prompt (`gemini.md`) that powers Atar.Bot, enabling systematic, evidence-based heritage assessments aligned with international standards.

---

## The `gemini.md` Prompt

The `gemini.md` file is a comprehensive AI instruction set that implements the full CBSA methodology. It contains:

- **6 Assessment Stages** (0–6): Pre-check, Contexts, Values, Authenticity/Integrity, Comparative Analysis, Significance Statement, Pulse Check
- **Structured Templates**: Ready-to-use frameworks for each stage
- **Context-Effect Framework**: Understanding two-way relationships between heritage and context
- **Built-in Quality Controls**: CSR (Cognitive Transparency), DQR (Dialogue Quality)
- **Knowledge Graph Generation**: Interactive visualization of heritage relationships
- **Multi-format Outputs**: Tables, timelines, comparative analysis, and more

---

## How to Use

### With Any AI Platform

You can use `gemini.md` with any AI system that supports long-context prompts:

1. **upload  the entire `gemini.md` file or use as GEM instructions**
2. **Paste it into your AI platform** 
3. **Upload your heritage documentation** (text, images, site plans)
4. **Start the assessment** by typing: "התחל בתהליך" (Hebrew) or "Start assessment" (English)

The AI will guide you step-by-step through the CBSA process, pausing for your input after each stage.

### Supported Platforms

- **Google Gemini** (recommended — designed for Gemini pro)
- **ChatGPT**  - plus models
- **Claude**  - 4.5 
- **DeepSeek**
- Any AI with large  context window

---

## Open Source & Customization

This project is **open source** and encourages adaptation:

✅ **Use freely** for heritage assessment projects  
✅ **Modify** stages, templates, or workflows to fit your needs  
✅ **Extract sections** for specific use cases (e.g., only Values assessment)  
✅ **Integrate** into your own tools or platforms  
✅ **Share improvements** back to the community (optional)

### License

MIT License — Free for academic, professional, and commercial use.

**Attribution:** Please credit the original authors when using or adapting this work.

---

## Credits

**Developed by:**

- **Associate Professor Yael Alef**, Heritage Methodology & CBSA Framework  
  📧 yaelalef@technion.ac.il

- **Yuval Shafriri**, AI Architecture & Implementation  
  📧 yuval.shafriri@gmail.com

**Workshop Context:** Developed for ICOMOS Israel Workshop, December 2024

---

## Quick Start Example

```markdown
User: "התחל בתהליך"
AI: [Runs Stage 0 Pre-check, identifies asset, lists available data, flags gaps]

User: "אשר מעבר לשלב 1"
AI: [Generates Stage 1: Contexts table with geographic, historical, social contexts + timeline]

User: "kg"
AI: [Creates interactive Knowledge Graph visualization in Canvas]
```

---

## Technical Notes

- **Context Window**: Requires AI with 128K+ tokens (1M+ recommended)
- **Language**: Bilingual (Hebrew/English) — mirrors user's language automatically
- **Output Formats**: Markdown tables, HTML (for Knowledge Graph), structured text
- **Human-in-the-Loop**: Pauses after each stage for user validation

---

## Support & Contributions

For questions, suggestions, or contributions:
- Open an issue in this repository
- Contact the authors directly (emails above)

---

**Last Updated:** December 2024  
**Version:** 2.0  
