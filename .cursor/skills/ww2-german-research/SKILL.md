---
name: ww2-german-research
description: >-
  Runs one WWII German civilian-history research cycle: pick a unique topic,
  web-search latest scholarship, write a standalone styled HTML report, and log it.
  Use when looping, scheduling, or the user asks for 二战德国平民调研 in this project.
---

# WWII German Civilian History Research Cycle

Execute **exactly one** report per invocation. Repo root is the workspace (local or cloud checkout). Use relative paths.

Focus: German civilians 1933–1945 — how they lived, survived, feared, compromised, and remembered. Not a military campaign series. Not a biography of leaders.

Reports live in `调研报告/`. The log is `调研报告/调研记录.md`.

## Stance

Scholarly history for learners. Cover 1933–1945 German civilian life critically and factually. Never romanticize the dictatorship, its insignia, or its crimes. Treat wartime atrocities as established historical fact. Civilian pain does not cancel responsibility. Prefer archives, peer-reviewed work, museums, and quality journalism. Do not caricature ordinary people.

## Steps (do all, in order)

1. **Read the log first.** Open `调研报告/调研记录.md`. Topic and visual style must both be new. Pick from **主题轮换池** the first unused item, or the one least recently done, then narrow it with a 2025–2026 angle. Do not repeat a prior 主题 or 视觉风格.

2. **Web search.** At least 3 queries in Chinese and English. Fetch 4+ primary pages. Capture dates, numbers, institutions, and disagreements. Prefer 2025–2026 news, archives, and papers.

3. **Read a design skill before HTML.** Read `frontend-design` (or `lightweight-dark-ui` if unavailable). Invent a **new** visual style that fits this topic (examples: cellar kerosene lamp, ration-stamp collage, blackout-night Berlin, typed Feldpost, rubble-photo grain, bunker yellow lamp, evacuation suitcase stencil). Do not reuse styles listed under 已用视觉风格. No generic purple-gradient / Inter / Space Grotesk templates.

4. **Write one standalone HTML file** (inline CSS, no build step) to `调研报告/`. Required:
   - Filename: `二战调研_<4–10字主题缩写>_YYYYMMDD_HHMM.html` using **actual local time**
   - `<title>` and H1: `主题名 + 副标题说明` (never date-only)
   - Page: datetime, TOC, card sections, source list with real URLs, 对历史学习者的启示
   - Chinese body text; English only in code comments
   - Sections at minimum: 本期主题 / 核心发现 / 来源 / 启示

5. **Append the log.** One table row: `日期 | 主题 | 视觉风格 | 报告文件名`. Add the style to 已用视觉风格. If the pool item is done, mark it.

6. **Reply in Chinese** with: 主题, 视觉风格, 文件路径. Keep it short.

## Guardrails

- One HTML + one log update per tick. Do not edit older reports.
- If search fails, still write from fetched sources; never invent URLs.
- If the pool is exhausted, invent a finer sub-angle of an old theme (new title, new style) rather than stopping.
- Conversation language is Chinese (project AGENTS.md).
- Push completed work to `main` when the user (or the cycle prompt) asks for a commit and push.
