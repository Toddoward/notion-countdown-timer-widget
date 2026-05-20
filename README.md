<div align="right">
  🌐 Read in: <a href="READMEmd" style="font-weight: bold;">English</a> | <a href="README.kr.md">한국어</a>
</div>

# Notion Countdown Timer Widget

<img width="1920" height="944" alt="image" src="https://github.com/user-attachments/assets/33ab6f66-4007-48a6-b416-0b8d51be0177" />

A simple, customizable countdown timer widget designed perfectly for Notion pages. This widget scales automatically to fit your Notion layout and is powered by the source code from [Logwork Countdown Timer](https://logwork.com/countdown-timer).

## 📂 Repository Structure

```text
notion-countdown-timer-widget/
├ README.md
├ README.kr.md
└ widget.html
```

## 🚀 How to Use
Follow these steps to create your own personalized countdown timer and embed it into Notion.

### 1. Fork this repository
Click the Fork button at the top right of this page to copy this repository to your own GitHub account.

### 2. Customize the settings
Open the `widget.html` file in your forked repository. Around line 42 inside the `<script>` tag, you will find the `countdownConfig` variable. Modify these values to set your own D-Day, title, and colors:

```js
const countdownConfig = {
  title: "UNIX Time Countdown",    // Widget Title Text
  date: "2038-01-19 12:14:07",     // D-day (YYYY-MM-DD HH:mm:ss)
  timezone: "Asia/Seoul",          // Timezone 
  language: "ko",                  // Language ISO 639-1 code(ex: en, es, fr, it, uk, pl, ru, de, ko, ja)
      colors: {
  colors: {
    text: "#6e6e6e",
    digits: "#ededed",
    units: "#8f8f8f"
  }
};
```

Commit the changes to your repository.

### 3. Deploy via GitHub Pages
1. Go to the `Settings` tab of your repository.

2. Click on `Pages` in the left sidebar.

3. Under `Build and deployment`, set the source to `Deploy from a branch` and select the `main` branch. Click `Save`.

4. After a minute or two, your widget will be live. Copy the link to your `widget.html` file (e.g., `https://your-username.github.io/notion-countdown-timer-widget/widget.html`).

### 4. Embed in Notion
1. Go to your Notion page.

2. Type `/embed` and select the Embed block.

3. Paste your GitHub Pages URL and click Embed link.

4. Drag the corners of the embed block to resize it. The timer will automatically scale to fit the container perfectly!

## 💡 Credits
This widget is built utilizing the countdown timer source code provided by [Logwork Countdown Timer](https://logwork.com/countdown-timer).
