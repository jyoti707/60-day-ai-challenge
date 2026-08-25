# 🧠 Content Intelligence Studio

### Day 47 — #60DayClaudeChallenge

An AI-powered content analysis platform that acts as a virtual editorial review desk. Content Intelligence Studio uses Claude to evaluate content through multiple specialized AI reviewers and turns their feedback into actionable recommendations.

## 🚀 Overview

Content Intelligence Studio helps creators understand how their content may perform before publishing.

Instead of relying on simple rule-based scoring, the application sends content to specialized Claude reviewers who analyze different dimensions of content quality.

The platform supports:

- 📝 Text content analysis
- 🖼️ Image analysis
- 🎯 Platform-specific recommendations
- 🧠 AI-powered reasoning
- ✍️ Content rewriting
- 🪝 Alternative hooks and titles
- 📊 Content health scoring
- 📈 AI-estimated performance potential
- ✅ Publishing checklist
- 🔍 Deeper optimization prompts

## ✨ Key Features

### Multi-Stage AI Review

The application automatically assembles a reviewer pipeline based on the uploaded content.

Specialized reviewers include:

- Hook & Opening Analyst
- Structure & Readability Editor
- Visual Content Analyst
- Distribution Strategist
- Engagement Psychology Reviewer
- Editor-in-Chief

Each reviewer has a dedicated system prompt and focuses on a specific aspect of content quality.

### 🖼️ Direct Image Analysis

Users can upload an image or screenshot along with their content.

Claude analyzes the actual visual content, including:

- Visual clarity
- Composition
- Text readability
- Professional polish
- Thumb-stop potential
- Relevance to the written content

### 📊 Content Health Dashboard

The final dashboard provides:

- Overall content score
- Category-level scores
- Strengths
- Weaknesses
- Missed opportunities
- Highest-impact improvements
- Platform-specific recommendations
- AI reasoning
- Predicted performance potential

### ✍️ AI Rewrite & Hooks

Claude can generate:

- A complete rewritten version
- Alternative hooks
- Alternative opening angles
- Stronger engagement opportunities
- Before-vs-after comparison

### 🔍 Publishing Checklist

The final report includes an AI-generated pre-publishing checklist to help creators improve the content before posting.

### 🤖 Deeper Optimization

The application generates additional prompts that can be used with Claude for further content optimization.

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Claude Messages API
- FileReader API
- Base64 image processing

No external frontend frameworks or libraries are required.

## 🔌 Claude API

The application uses the Claude Messages API:

`https://api.anthropic.com/v1/messages`

The application sends content directly to Claude for analysis and receives the reviewer insights through live API calls.

The project intentionally avoids:

- Hardcoded content scores
- Canned feedback
- Placeholder analysis
- Rule-based editorial scoring
- JSON-based reviewer output

Reviewer responses use structured plain-text sections to make parsing more resilient.

## 🧩 Architecture

```text
User Content
     │
     ├── Text
     │
     └── Image
          │
          ▼
   Content Intelligence
        Pipeline
          │
          ▼
 ┌───────────────────────┐
 │ Hook Analyst          │
 │ Structure Editor      │
 │ Visual Analyst        │
 │ Distribution Strategist│
 │ Psychology Reviewer   │
 └───────────────────────┘
          │
          ▼
    Editor-in-Chief
          │
          ▼
   Final AI Report
          │
          ├── Overall Score
          ├── Strengths
          ├── Weaknesses
          ├── Opportunities
          ├── Recommendations
          ├── Rewrite
          ├── Alternative Hooks
          ├── Performance Estimate
          ├── Publishing Checklist
          └── Deeper Prompts
