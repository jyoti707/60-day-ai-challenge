# ⚖️ The Verdict Engine — Compare & Decide

A research-driven decision-support tool that helps users make better choices by comparing real-world options across measurable criteria.

Built for **Day 48 of the 60-Day Claude Challenge**.

## 🚀 What It Does

The Verdict Engine turns a complicated comparison into a personalized ranking.

For this version, I built a **laptop comparison engine** for students and budget-conscious buyers. Users can adjust how important each criterion is and instantly see the ranking change.

### ✨ Key Features

* 🎯 **Personalized criteria weighting**
* 📊 **Live ranking calculation**
* 💻 Comparison of multiple laptops
* 💰 Price comparison
* 🔋 Battery-life comparison
* ⚖️ Weight comparison
* ⚡ Performance comparison
* 📚 Visible sources & citations
* ⚠️ Clear labeling of estimated data
* 🔎 "How this was researched" section
* 📖 Explanation of conflicting sources
* 🔄 Preset decision profiles:

  * Tight Budget
  * Travel
  * Performance
  * Balanced
* 📱 Fully responsive design
* 🛡️ Graceful loading and empty states
* 🔒 No data is sent anywhere

## 🧠 How The Ranking Works

Each laptop is scored against every criterion and the values are normalized to a **0–100 scale**.

Users assign each criterion a weight from **0–10**.

The final score is calculated as a weighted average:

**Final Score = Σ(Normalized Criterion Score × Weight) / Σ(Weights)**

This means the "best" laptop isn't necessarily the same for everyone.

A budget-focused user can get a different winner from someone who prioritizes performance or portability.

## 🔬 Research Approach

The comparison uses named sources including manufacturer specifications and independent technology reviews.

Where sources disagree, the application explicitly explains the conflict rather than silently hiding it.

For example, battery life can differ significantly between manufacturer claims and independent testing, so estimated figures are clearly marked in the interface.

## 💻 Technologies

* HTML
* CSS
* Vanilla JavaScript

No external libraries or frameworks are required.

## 🎯 Challenge

**60-Day Claude Challenge — Day 48**

> Build The Verdict Engine
> *The AI That Renders a Verdict on Your Toughest Decisions*

The goal was to create a decision-support experience that combines research, data visualization, and interactive weighting into one practical tool.

## 📌 Current Comparison

The current version compares:

* MacBook Air M3
* Dell XPS 13 9345
* Lenovo ThinkPad X1 Carbon Gen 12
* ASUS ZenBook 14 OLED

The underlying data and citations are displayed directly inside the application.

## 📂 Project Structure

```text
laptop-compare.html
```

The entire application is contained in a single HTML file with embedded CSS and JavaScript.

## 🌟 Why I Built It

Instead of simply saying **"Laptop A is better than Laptop B,"** the goal was to answer:

**"Which option is better for YOU, based on what YOU value?"**

That shift from a fixed comparison to a personalized decision engine is the core idea behind this project.
