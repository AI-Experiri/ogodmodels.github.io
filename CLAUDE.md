# CLAUDE.md - Hacker News Story Selection Guidelines

## Overview

This document specifies how to select Hacker News stories for the OHGOD Philosophy website's problem cards. Each problem card has a flip animation that reveals 4 HN stories on the back.

## Requirements for HN Stories

### Minimum Engagement
- Each story MUST have at least **100 comments** on Hacker News
- Stories with 200+ comments are preferred
- Major announcement posts (GPT-4, Mamba, etc.) typically have 300+ comments

### Story Selection Criteria

1. **First Story Must Support the Stat**
   - The statistic shown on the front of the card must be directly mentioned or supported by the first story
   - Example: If stat is "$100M+", the first story should discuss GPT-4 training costs of $100M

2. **Variety of Sources**
   - Avoid multiple stories about the same company incident (e.g., don't use 3 Samsung stories)
   - Mix different angles: research papers, news, lawsuits, Ask HN discussions

3. **Landmark/Viral Stories Preferred**
   - Major product announcements (GPT-4, GPT-4o, Mamba)
   - Viral incidents (Samsung data leak)
   - Major lawsuits (NY Times vs OpenAI)
   - Research papers that went viral

4. **Recency**
   - Prefer stories from 2023-2025
   - Older stories acceptable if they're landmark discussions

## How to Find High-Engagement Stories

### Search Strategy
```
site:news.ycombinator.com [topic] [year]
```

### Verify Comment Count
- Visit the HN link directly
- Check the comment count at the top
- Stories with 100+ comments usually have significant discussion

### Popular Story Indicators
- Major tech announcements
- Controversial topics
- Research paper releases
- Corporate scandals/leaks
- Lawsuits involving Big Tech

## Current Problem Cards and Their Stories (Updated Dec 2024)

### Problem 1: Power Concentrated ($10B)
- Elon Musk Spent $10B on AI Training Hardware in 2024 (Oct 2024)
- AI Models That Cost $1B to Train Are Underway (Jul 2024)
- U.S. Antitrust Inquiries (Jun 2024)
- AI Training Costs Increasing 3x Annually (Aug 2025)

### Problem 2: Planet Can't Afford (900k tons CO₂)
- AI Adoption in US Adds ~900k Tons CO₂ Annually (2025 study)
- Big Tech AI Data Centers Driving Up Bills (Aug 2025)
- AI, but at What Cost? Carbon Footprint Breakdown (Feb 2025)
- Google's Carbon Emissions Surge 50% (Jul 2024)

### Problem 3: Data Isn't Yours (20M+ conversations)
- Fighting NYT's Invasion of User Privacy (2025) - 20M+ stored chats
- Why is OpenAI Lying About Data Collection? (2025)
- OpenAI Slams Order to Save All ChatGPT Logs (Jun 2025)
- NY Times Suing OpenAI for Copyright (Jan 2024)

### Problem 4: Nobody Knows Inside (0%)
- GPT-4 (Mar 2023) - 0% architecture disclosed
- GPT-4 Details Leaked? (Jul 2023)
- GPT-4o (May 2024)
- GPT-4.5 (Feb 2025)

### Problem 5: Illusion of Intelligence (covers sycophancy + hallucination + memorization)
- Sycophancy Is the First LLM 'Dark Pattern' (2025)
- Claude Says 'You're Absolutely Right!' About Everything (Aug 2025)
- Hallucination Is Inevitable: Innate LLM Limitation (Feb 2024)
- LLMs Regurgitating Training Data (May 2024) - memorization

### Problem 6: Architecture Barely Changes (8 yrs)
- 'Attention Is All You Need' Coauthor 'Sick' of Transformers (Oct 2025)
- Ask HN: Is Anybody Building Alternative Transformer? (Feb 2025)
- How Has DeepSeek Improved Transformer Architecture? (Jan 2025)
- Mamba: Linear-Time Sequence Modeling (Dec 2023)

## Story Format in HTML

```liquid
story1_url="https://news.ycombinator.com/item?id=XXXXXXXX"
story1_title="Title (max ~50 chars)"
story1_summary="One-line summary (max ~50 chars)"
```

## Updating Stories

When updating stories:
1. Search for high-engagement HN discussions on the topic
2. Verify 100+ comments
3. Ensure first story supports the card's statistic
4. Maintain variety across the 4 stories
5. Keep titles and summaries concise for card display

# Git Commit Rules (MANDATORY)

1. NEVER add "Co-Authored-By:" lines to commits
2. NEVER add "🤖 Generated with [Claude Code]" to commits
3. Keep commit messages simple and descriptive
4. Just describe what changed - no AI attribution footer
