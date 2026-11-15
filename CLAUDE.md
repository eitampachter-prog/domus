# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Domus is an academic product project: a mobile app for roommates that documents chores with photos, has AI estimate the effort, and awards points once completion is verified. The MVP is points only, with no money. The spec ("אפיון אפליקציה", 25.10.2026) defines Phase 1 (Discovery) and Phase 2 (UX/UI in Google Stitch).

This folder has no code. The deliverable is a **Google Stitch prototype**, built through the Stitch MCP server (`mcp__stitch__*`).

## Stitch project

- Project: `projects/11405005407106127418`, titled "Domus – אב טיפוס"
- Design system: `assets/4786086149755272388`, "Domus Cyber-Home". Pass it as `designSystem` on every `generate_screen_from_text` call, with `deviceType: MOBILE`.
- Visual language:
  - Font: Rubik.
  - Colors: indigo `#3D2FB0` for primary actions, mint `#2EC4A0` for points, karma and success, coral `#FF6B5B` for errors, amber `#FFB020` for pending and review.
  - Rounded cards. Status chips always carry an icon and text, never color alone.
- Bottom tab bar, ordered from the right: בית, לוח מטלות, raised + button, נקודות, פרופיל.

## Prototype rules (decided with the user)

- **Language:** the whole UI is in Hebrew and fully RTL (`dir="rtl"`). Every prompt must restate this, or Stitch drifts into English or LTR.
- **Sample data:** keep it identical on every screen.
  - Household "דירת הרצל 12"; members נועה (current user, 120 נק׳), איתי (95), מאיה (80).
  - Flagship task "ניקוי יסודי של האמבטיה", worth 35 points: published by נועה, claimed by איתי. After verification, איתי's balance goes 95 → 130.
  - Other tasks: "קניות שבועיות בסופר" (25), "תשלום ארנונה" (20, claimed by מאיה).
- **Points table:** ניקיון 10/20/35, קניות 10/15/25, חשבונות 15/20/30, for low/medium/high complexity. The user may adjust one level before publishing. Points never grow over time.
- **Claiming:** the publisher can't claim their own task. A claimed task can be released back to the board. Appeals go to a review queue, decided by another member or the house admin.
- **Tone:** never judgmental toward roommates.

## Required screens

- Main flow: onboarding, sign-up, create/join home, dashboard, Before camera, AI scan, AI result & confirm points, chore board, task details, After photo, verification success, points ledger, household activity, profile/settings.
- Alternate path and system states (spec section 11.4): retake needed, not approved (resubmit/appeal), review queue plus a review detail screen, empty board, upload failed, camera permission denied, task already claimed.

## Stitch MCP quirks

- `generate_screen_from_text` usually **times out client-side but still succeeds** server-side, taking several minutes. Don't retry. Wait in the background (`sleep` with `run_in_background`), then check with `list_screens`.
- On 2026-11-15, after the first 2 screens, no new screens appeared, whether sent in parallel or alone. With `GEMINI_3_5_FLASH_LITE`, the call returns quickly with a "screen created" message but creates no screen. Always confirm with `list_screens`. Every screen prompt is in `stitch-prompts.md`.
- The first dashboard prompt was sent twice, so the project holds two dashboard screens. One should be hidden or removed.
- The MCP has no tool for prototype links (hotspots). Wire click-throughs manually in Stitch's Prototype mode.
- Python and Node are not installed. To view a screenshot, use PowerShell: read the saved `download_file` JSON, `[Convert]::FromBase64String($j.image)`, and resize with `System.Drawing`.
