# TalentLens-WakePing 🚀

[![Keep TalentLens Awake](https://github.com/FrankOlum/TalentLens-WakePing/actions/workflows/ping.yml/badge.svg)](https://github.com/FrankOlum/TalentLens-WakePing/actions)

A lightweight utility repo designed to keep the [TalentLens Hugging Face Space](https://huggingface.co/spaces/FrankOlum/TalentLens) responsive.

## Purpose
Hugging Face Spaces go to sleep 😴 after periods of inactivity. This repo uses a GitHub Actions workflow to send periodic requests, ensuring TalentLens stays awake and visitors don’t encounter the default “wake up” banner.

## How It Works
- **Scheduled pings**: A workflow runs every 20 minutes, silently requesting the Space URL.
- **Manual trigger**: You can wake the Space instantly via the GitHub Actions tab.

## Repo Structure
- `README.md` → Documentation (this file).
- `.github/workflows/ping.yml` → Workflow definition for scheduled + manual pings.

## Notes
- This repo does not contain the TalentLens app code — only a keep-alive mechanism.
- Safe, minimal, and effective: two files are all that’s needed.