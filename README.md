# Chat Analyzer

A **Streamlit-based WhatsApp chat analysis tool** that provides detailed insights about chat activity, messages, emojis, most common words, timelines, and word clouds. Supports Hindi-English (Hinglish) stopwords filtering.

---

## Table of Contents
- Overview
- Features
- Installation
- Usage
- Files
- License

---

## Overview

Chat Analyzer processes exported WhatsApp chat files and provides visual and statistical insights. It can analyze individual users or the entire group chat. Key functionalities include media and link counts, emoji analysis, word frequency, monthly/daily timelines, activity heatmaps, and word clouds.

---

## Features

- Parse WhatsApp chat `.txt` files
- Preprocess messages and timestamps
- Compute chat statistics:
  - Total messages
  - Total words
  - Media shared
  - Links shared
  - Deleted messages
- User activity analysis (daily, weekly, monthly)
- Emoji usage analysis
- Most common words in the chat (Hinglish stopwords filtered)
- Monthly and daily timelines
- Wordcloud generation
- Weekly activity heatmap
- Interactive Streamlit interface

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/shaunak-alt/chat-analyzer.git
```

2. Install required Python packages:

```bash
pip install pandas numpy matplotlib seaborn streamlit urlextract emoji wordcloud
```

---

## Usage

1. Run the Streamlit app:

```bash
streamlit run main.py
```

2. Upload your exported WhatsApp chat file (`.txt`) when prompted.

3. Select date format (`dd-mm-yy` or `mm-dd-yy`) and user to analyze from the sidebar.

4. Click **Show Analysis** to view detailed statistics, timelines, emoji analysis, word clouds, and heatmaps.

---

## Files

- `main.py` – Main Streamlit app for interactive chat analysis.
- `functions.py` – Helper functions for data parsing, preprocessing, analysis, and visualization.
- `stop_hinglish.txt` – List of common Hindi-English stopwords for text processing.
