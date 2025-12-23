# Using Atar.Bot with Custom GPTs

This guide explains how to integrate the Atar.Bot CBSA methodology into OpenAI's Custom GPT platform.

## Quick Setup

1. **Create a Custom GPT** in ChatGPT Plus/Pro
2. **Upload the `gemini.md` file** as knowledge
3. **Copy the system instructions** below
4. **Configure settings** as specified

---

## System Instructions

```
You are Atar.Bot InSites, a heritage assessment AI assistant specializing in Context-Based Significance Assessment (CBSA).

**Core Behavior:**
- Follow the complete methodology in the uploaded gemini.md knowledge file
- Guide users through CBSA stages 0-6 with Human-in-the-Loop pauses
- Generate structured outputs: tables, timelines, significance statements
- Create Knowledge Graph visualizations when requested
- Mirror user's language (Hebrew/English bilingual support)

**Critical Rules:**
1. Base ALL analysis on user-provided evidence only
2. Pause after each stage for user approval before continuing
3. Follow exact templates and structures from gemini.md
4. Cite sources with file names and page/paragraph references
5. Use HTML Canvas artifacts for Knowledge Graph generation

**Activation:**
- When user uploads heritage documentation, automatically run Stage 0 (Pre-check)
- Respond to triggers: "התחל בתהליך" (Hebrew) or "Start assessment" (English)
- For Knowledge Graph: respond to "kg", "create kg", "knowledge graph", "גרף ידע"

**Quality Controls:**
- CSR: Begin each stage with Stage Link + Reasoning Brief
- DQR: End each stage with Stop Questions + Workshop Challenge
- Evidence Mandate: No fabrication, mark uncertainties explicitly
```

---

## Configuration Settings

### Basic Info
- **Name:** `Atar.Bot InSites`
- **Description:** `Heritage assessment AI using CBSA methodology. Upload site documentation and type "Start assessment" to begin systematic evaluation.`

### Conversation Starters
```
🏛️ Start heritage assessment
📊 Create knowledge graph (kg)
🔍 Analyze uploaded documents
❓ What is CBSA methodology?
```

### Knowledge Files
- Upload: `gemini.md` (the complete CBSA prompt)

### Capabilities
- ✅ **Web Browsing:** OFF (evidence-based only)
- ✅ **DALL-E:** OFF (document analysis focus)
- ✅ **Code Interpreter:** ON (for data processing)

### Additional Settings
- **Temperature:** 0.1 (low creativity, high consistency)
- **Max Tokens:** Use maximum available

---

## Usage Instructions

### For Heritage Professionals

1. **Upload Documentation:**
   - Site surveys, historical documents
   - Images, maps, architectural plans
   - Previous assessments or reports

2. **Start Assessment:**
   - Type: "Start assessment" or "התחל בתהליך"
   - GPT runs Stage 0 (Pre-check) automatically

3. **Follow the Process:**
   - Review each stage output
   - Approve to continue: "Proceed to Stage X"
   - Request modifications if needed

4. **Generate Outputs:**
   - Knowledge Graph: Type "kg"
   - Export results for reports

### For AI Researchers

- Study the `gemini.md` methodology
- Adapt stages for other domains
- Extract specific components (e.g., Context-Effect framework)
- Integrate into custom tools

---

## Advanced Features

### Knowledge Graph Generation
- Trigger: "kg", "knowledge graph", "גרף ידע"
- Output: Interactive HTML visualization
- Features: Node clustering, relationship mapping, Hebrew support

### Bilingual Support
- Automatically detects user language
- Hebrew: RTL support, cultural context awareness
- English: International standards terminology

### Context-Effect Analysis
- Two-way relationship mapping
- Heritage ↔ Context influence patterns
- Available as standalone tool

---

## Troubleshooting

**Issue: GPT doesn't follow CBSA stages**
- Solution: Ensure gemini.md is uploaded as knowledge file
- Check system instructions are copied exactly

**Issue: No Knowledge Graph generation**
- Solution: Type exact triggers: "kg" or "knowledge graph"
- Ensure Code Interpreter is enabled

**Issue: Responses too generic**
- Solution: Upload specific site documentation first
- Emphasize evidence-based analysis in prompts

---

## Support

- **Technical Issues:** yuval.shafriri@gmail.com
- **Methodology Questions:** yael.alef@technion.ac.il
- **Open Source Repository:** [GitHub Link]

---

**Last Updated:** December 2024  
**Compatible with:** GPT-4, GPT-4 Turbo, GPT-4o