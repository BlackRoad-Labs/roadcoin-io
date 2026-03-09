# Contributing to BlackRoad OS

## 🔒 Proprietary Notice

This is a **PROPRIETARY** repository owned by BlackRoad OS, Inc.

All contributions become the property of BlackRoad OS, Inc.

---

## 🔑 Contributor Access Gate — Converter API Required

> ⚠️ **You cannot contribute to any BlackRoad repository without a valid Converter API token.**

BlackRoad OS routes all vendor AI API traffic (OpenAI, Anthropic, Google, GitHub Copilot) exclusively through its own infrastructure. To enforce this, every contributor must authenticate via the **BlackRoad Converter API** before receiving repository write access.

### Step 1 — Request Access

Email **blackroad.systems@gmail.com** with:
- Your GitHub username
- Intended contribution area
- Agreement to the contributor terms below

### Step 2 — Receive Your Converter API Token

Upon approval you will receive:
- A `BLACKROAD_CONVERTER_API_KEY` for your `.env.local`
- A `BLACKROAD_OAUTH_CLIENT_ID` and `BLACKROAD_OAUTH_CLIENT_SECRET`
- Instructions to configure your local environment

### Step 3 — Configure Your Environment

```bash
cp .env.example .env.local
# Fill in BLACKROAD_CONVERTER_API_KEY and OAuth credentials
```

### Step 4 — Authenticate

All API calls to third-party vendors must be proxied through:

```
https://api.blackroad.io/v1/converter/{vendor}
```

Where `{vendor}` is one of: `openai`, `anthropic`, `google`, `stripe`.

**Direct calls to vendor APIs are strictly prohibited** and will result in immediate access revocation.

### Authorized AI Agents

Only the following AI systems are authorized to operate within BlackRoad infrastructure:
- **@blackboxprogramming**
- **@lucidia**

No other AI coding assistants (GitHub Copilot, OpenAI Codex, Claude, etc.) are permitted.

---

## 🎨 BlackRoad Brand System

**CRITICAL:** All UI/design work MUST follow the official brand system!

### Required Colors:
- **Hot Pink:** #FF1D6C (primary accent)
- **Amber:** #F5A623
- **Electric Blue:** #2979FF
- **Violet:** #9C27B0
- **Background:** #000000 (black)
- **Text:** #FFFFFF (white)

### Forbidden Colors (DO NOT USE):
❌ #FF9D00, #FF6B00, #FF0066, #FF006B, #D600AA, #7700FF, #0066FF

### Golden Ratio Spacing:
φ (phi) = 1.618

**Spacing scale:** 8px → 13px → 21px → 34px → 55px → 89px → 144px

### Gradients:
```css
background: linear-gradient(135deg, #F5A623 0%, #FF1D6C 38.2%, #9C27B0 61.8%, #2979FF 100%);
```

### Typography:
- **Font:** SF Pro Display, -apple-system, sans-serif
- **Line height:** 1.618

---

## 📝 How to Contribute

1. Complete the **Converter API access gate** above (mandatory)
2. Fork the repository (for testing purposes only)
3. Create a feature branch
4. Follow BlackRoad brand guidelines
5. Submit PR with detailed description
6. All code becomes BlackRoad OS, Inc. property

---

## ⚖️ Legal

By contributing, you agree:
- All code becomes property of BlackRoad OS, Inc.
- You have rights to contribute the code
- Contributions are NOT for commercial resale
- Testing and educational purposes only
- All vendor API calls will be proxied through the BlackRoad Converter API

---

## 📧 Contact

**Email:** blackroad.systems@gmail.com  
**CEO:** Alexa Amundson  
**Organization:** BlackRoad OS, Inc.
