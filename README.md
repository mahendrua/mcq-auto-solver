# MCQ Auto Solver with GitHub Copilot

A Chrome extension that automatically solves multiple-choice questions (MCQ) using GitHub Copilot API.

## Features

✅ **Automatic Question Extraction** - Reads questions and options from quiz pages
✅ **GitHub Copilot Integration** - Uses Copilot API to determine correct answers
✅ **Auto-Navigation** - Automatically clicks Next button to proceed
✅ **Works on Most Platforms** - Google Forms, Quizzes, and custom quiz platforms
✅ **Configurable Delays** - Adjust timing between actions
✅ **Real-time Logging** - Track progress in the popup

## Installation

### Step 1: Clone or Download
Clone this repository or download as ZIP

### Step 2: Load Extension in Chrome
1. Open Chrome and go to `chrome://extensions/`
2. Turn on **Developer mode** (toggle in top-right corner)
3. Click **Load unpacked**
4. Select the `mcq-auto-solver` folder
5. The extension will appear in your toolbar

### Step 3: Get GitHub Copilot API Token
1. Go to https://github.com/settings/tokens
2. Click **Generate new token (classic)**
3. Select scopes: `copilot`, `admin:repo_hook`
4. Copy the token

## Usage

1. **Open a Quiz** - Navigate to any MCQ quiz in Chrome
2. **Click Extension Icon** - Click the MCQ Auto Solver icon in toolbar
3. **Enter API Token** - Paste your GitHub token in the token field
4. **Save Settings** - Click "Save Settings"
5. **Start Solving** - Click "▶ Start Solving" button
6. **Monitor Progress** - Watch the log for real-time updates
7. **Stop Anytime** - Click "⏹ Stop" to pause

## Configuration

- **GitHub Copilot Token**: Your personal access token with Copilot scope
- **Delay (ms)**: Time between actions (default: 1500ms)
  - Lower = faster (min 500ms)
  - Higher = slower (max 5000ms)

## How It Works

1. **Content Script** - Scans the page for questions and multiple-choice options
2. **Background Worker** - Sends question to GitHub Copilot API
3. **Auto-Click Logic** - Clicks the correct answer and navigates to next question

## Supported Quiz Platforms

- ✅ Google Forms
- ✅ Quizlet
- ✅ Canvas Quiz
- ✅ Moodle
- ✅ Custom quiz platforms

## Legal Notice

⚠️ **Use Responsibly**: This extension is for educational purposes. Check your institution's academic integrity policy before using on graded assessments.