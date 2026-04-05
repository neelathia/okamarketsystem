# OKA Market System — Setup Reference

## What this system does
Processes raw job postings into structured market intelligence 
and publishes them to GitHub automatically.

## Pipeline
Paste JD to Claude → Claude structures it → 
Save in Obsidian (02_Structured) → 
Auto-syncs to GitHub every 10 min → 
Claude reads anytime from GitHub

## Folder Structure
01_Raw        → unprocessed signals (screenshots, raw JDs)
02_Structured → structured JD analysis (JP– files)
03_Insights   → your thinking (patterns, positioning)
04_Proof      → your stories (TTX, case studies)

## GitHub Repo
https://github.com/neelathia/okamarketsystem

## Claude Project
All JD processing happens inside this Project.
Start a new chat inside the Project each session.
Claude rebuilds the artifact on request.

## JD Processing Steps
1. Paste raw JD into Claude
2. Claude structures it using JP– template
3. Copy structured output into Obsidian → 02_Structured
4. Obsidian Git auto-pushes to GitHub every 10 minutes

## File Naming Convention
JP___Role_Name___Layer___SignalStrength.md

Layer = Execution / System / Architecture
Signal Strength = Very High / High / Medium / Low

## Template Location
02_Structured/STRUCTURED_Template.md

## Obsidian Git Plugin Settings
Auto commit interval: 10 minutes
Auto push interval: 10 minutes
Commit message: vault backup: {{date}}

## GitHub Token
Generate at: github.com/settings/tokens
Scope needed: repo
Rotate token regularly — never share in chat

## To rebuild the JD processor artifact
Start new chat in this Project and say:
"Rebuild my JD processor artifact"

## Claude can read your vault anytime
Share this URL in any Project conversation:
https://github.com/neelathia/okamarketsystem
Claude will fetch files directly — no pasting needed