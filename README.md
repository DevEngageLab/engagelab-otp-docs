# EngageLab Official Documentation

This repository contains the official documentation for **EngageLab**, including comprehensive guides, API references, and SDK instructions for the EngageLab OTP service and other products. 

The documentation site is built using [Mintlify](https://mintlify.com/).

## 🚀 Local Development

To preview the documentation locally, you need to install the Mintlify CLI.

### 1. Install Mintlify CLI
```bash
npm i -g mintlify
```

### 2. Run the Development Server
Run the following command at the root of the repository (where `docs.json` is located):
```bash
mint dev
```
Your local preview will be available at `http://localhost:3000`.

### 3. Check for Broken Links
Before committing your changes, you can verify that all internal links are working correctly:
```bash
mint broken-links
```

## 📁 Project Structure

- `docs.json`: The core configuration file for the site's navigation, theme, SEO, and global settings.
- `otp/`: Documentation specific to the EngageLab OTP service.
  - `getting-started/`: Overview, quickstart, and AI onboarding guides.
  - `api/`: OpenAPI 3.0.1 JSON schemas and detailed API reference pages.
  - `ways-to-use/`: Integration guides for REST APIs, SDKs (Node.js & Python), and AI Agent Skills.

## ✍️ Writing Guidelines

- **Format:** All documentation pages are written in MDX (`.mdx`) and require YAML frontmatter.
- **Icons:** We use [Lucide icons](https://lucide.dev/icons/) for the `icon` field in the frontmatter and Mintlify components (e.g., `<Card>`, `<Step>`).
- **API References:** API documentation is generated from OpenAPI 3.0.1 JSON schemas located in the `otp/api/` directory. The `x-mint.href` property is used in the JSON schemas to map endpoints to their respective URLs.

## 🤖 AI-Assisted Writing

If you are using AI coding tools (like Cursor, Claude Code, or Windsurf) to contribute to this documentation, you can install the Mintlify documentation skill to provide your AI agent with component references and writing standards:

```bash
npx skills add https://mintlify.com/docs
```

## 🌐 Links

- [EngageLab Official Website](https://www.engagelab.com/)
- [EngageLab Console](https://www.engagelab.com/console/)