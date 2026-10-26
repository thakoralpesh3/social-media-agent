# 📱 Autonomous AI Social Media Agent

[![Daily Social Media Agent](https://github.com/thakoralpesh3/social-media-agent/actions/workflows/daily_social_agent.yml/badge.svg)](https://github.com/thakoralpesh3/social-media-agent/actions/workflows/daily_social_agent.yml)

Autonomous AI multi-platform social story creator and syndicator. Generates and publishes daily trilingual stories and status updates across **Instagram, Facebook, and WhatsApp** every day at **09:00 AM IST**.

---

## ⚡ Core Features
- **Trilingual Story Generation**: Autonomous story generation across English, Hindi (Devanagari), and Gujarati.
- **Multilingual Voiceovers**: Edge neural TTS voices tailored per language.
- **Visual Story Scenes**: Vertical 9:16 story cards & animated video scenes with automatic subtitle overlays.
- **Multi-Platform Syndication**:
  - 📸 **Instagram**: Direct story and reels publishing.
  - 📘 **Facebook**: Direct page story and video publishing.
  - 💬 **WhatsApp**: Automatic HTML5/Web status dispatch.
- **100% Cloud-Autonomous**: Runs inside GitHub Actions daily at **09:00 AM IST** with zero laptop dependency.

---

## 🚀 Running on GitHub Actions
The agent runs automatically on GitHub Actions every day at **09:00 AM IST** (`cron: '30 3 * * *'`).

You can also trigger it on demand:
1. Navigate to **Actions** > **Daily Social Media Agent Workflow**.
2. Click **Run workflow**.
3. Choose options:
   - `content_source`: `generate`, `post_folder`, or `both`.
   - `topic`: Custom topic (or leave empty for autonomous daily selection).
   - `dry_run`: `true` or `false`.

---

## 🔐 Required GitHub Secrets
Configure these in **Settings** > **Secrets and variables** > **Actions**:
- `GEMINI_API_KEY`: Google Gemini API key.
- `SOCIAL_CREDENTIALS_JSON`: WhatsApp, Instagram, and Facebook credentials & sessions.
