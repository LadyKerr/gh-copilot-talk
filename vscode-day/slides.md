---
theme: seriph
title: Beyond the Editor - tips to get the most out of GitHub Copilot
background: https://github.com/LadyKerr/try-streamlit/assets/47188731/1af40df6-89a8-41bd-b7e0-dfa48682e652
favicon: ''
font: Playfair Display
layout: cover
lineNumbers: true
transition: fade
record: dev
download: true
exportFilename: gh-copilot-vscode
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
---

<!--
Hello good morning! Thank you all for being here with me today to learn how to get the most ourt of GitHub Copilot.
-->

---
layout: image-right
image: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/7d0e2430-c5c9-483a-b8eb-afcda71e80f8
transition: fade-out
---

# Hi! I'm Kedasha!

- Jamaican gyal! 🇯🇲 
- Developer Advocate at GitHub 
- Software Developer for ~4 years 
- Technical Content Creator ✨ 
- Committed to teaching and learning in public

<br>

I love, love, love creating technical content on Instagram, Tiktok and sometimes Twitter. 

**Find me online @itsthatladydev**

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


<!--

Hello! I'm Kedasha Kerr and Im a Developer Advocate at GitHub. 

Im super excited to talk to you about GitHub Copilot and how to get the most out of this tool. We know the tool, we love the tool, but how do we make GitHub Copilot work for us more effectively?

Today, I'll be sharing some pragmatic ways to get the most out of GitHub Copilot during your day to day development.
-->


---
layout: intro
transition: fade-out
---

# What we'll cover:

- Brief Overview of GitHub Copilot
- Tips for using GitHub Copilot + VS Code 
- Going Beyond your Editor 
- Live Demo 
- Q&A and Resources 


<img src="https://github.com/LadyKerr/try-streamlit/assets/47188731/498d8d32-a686-4287-a6ce-d3b774d3a4ce" width="500px" height="500px" />

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<div class="absolute left-30px bottom-30px">
@itsthatladydev
</div>

<!--
We'll take a brief look at what GitHub Copilot is, tips to get the most out of it, and then we'll do some live demos.

Let's jump right into it!
-->

---
layout: intro
transition: fade-out
---

# GitHub Copilot

### The world's most widely adopted AI developer tool ✨

<br />
<br />

<img src="https://github.com/LadyKerr/try-streamlit/assets/47188731/00eefc9c-a3ae-4538-a574-6f6ed69112d8" alt="github copilot in vscode" />

<style>
h1 {
  background-color: #40C9FF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--

But first, what is GitHub Copilot? :thinking:

Just in case you didn't know, GitHub Copilot is an AI pair programmer that helps you write code faster. It is designed to help with programming tasks and serves as your assistant while you're working in your IDE.

-->

---
transition: fade-out
layout: intro
---

# GitHub Copilot + VS Code Tips

```python {5-6|7-8|9-10|11-12|13-15|all}{lines:true, startLine:5}
def vscode_copilot_tips():
  tips = {
    'agent': '@workspace',
    'reference': '#file',
    'sparkles': 'keep a lookout for ✨ in your editor',
    'terminal_help': 'gh-copilot in your terminal to help with debugging',
    'remove_chat': 'remove irrelevant conversations from Chat',
    'quick_actions': 'slash commands for quick actions',
    'commit_messages': 'Copilot to write commit messages',
    'inline_chat': 'inline chat',
    'enable_disable': 'enable/disable copilot anytime and for specific languages'
  }
  return tips
```

<!--

- Use @workspace agent
- Use #file to attach files for reference
- look for Sparkles throughout the editor
- Copilot in your terminal to help with debugging
- remove irrelevant conversations from Chat
- slash commands for quick actions
- Copilot to write commit messages
- inline chat
- enable/disable copilot anytime and for specific languages

-->

<style>
h1 {
  background-color: #40C9FF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<div class="absolute left-30px bottom-30px">
@itsthatladydev
</div>

---
transition: fade-out
layout: intro
---

# Beyond the Editor

### GitHub Copilot extends beyond your editor - it is in the CLI, on your mobile phone and on GitHub dotcom!
<br />

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<div class="absolute left-30px bottom-30px">
@itsthatladydev
</div>

<!--

Some of the tools that accompany GitHub Copilot includes a chat interface that you can use in your IDE, a command line tool via a GitHub CLI extension, GitHub Copilot for PRs, Copilot integrated into dotcom and many more. Today, we'll be looking at a few of the features that I've found to be most useful during my everyday development.

-->

---
layout: section
transition: fade-out
---

# Let's take a look!

### demo repo: **gh.io/streamlit**

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<div class="absolute left-30px bottom-30px">
@itsthatladydev
</div>

<!--

DEMO Doc: https://docs.google.com/document/d/1lEopGEH58CZl5BXf8f5Sie0ZXBtefWELFsCuHq8hXqQ/edit?usp=sharing 

-->

---
layout: quote
transition: fade-out
---

# Remember:

## To make the most  out of GitHub Copilot is to know all the features that are available to you.

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<div class="absolute left-30px bottom-30px">
@itsthatladydev
</div>


---
transition: fade-out
---

# Learn more on the blog:

<br />

<div style="display: flex;">
  <div style="flex: 50%; padding: 10px;">
    <img src="https://github.com/LadyKerr/gh-copilot-talk/assets/47188731/cdea8189-2db9-4c51-9e67-281278312cf2" alt="using-copilot-tips" height="200" width="400">
  </div>
  <div style="flex: 50%; padding: 10px;">
    <img src="https://github.com/LadyKerr/gh-copilot-talk/assets/47188731/019dab54-13fe-4e79-8e13-a03dacf531e4" alt="using-copilot-tips" height="200" width="400">
  </div>
</div>

- **Demo and resources:** - gh.io/streamlit

<br>

**@itsthatladydev**
<br>
Find me on all socials!

<style>
h1 {
  background-color: #40C9FF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: section
transition: fade-out
---
# Thank you!

### 👉🏽 **gh.io/streamlit**
<br />
<br />

#### @itsthatladydev

<style>
h1 {
  background-color: #E81CFF;
  background-image: linear-gradient(45deg, #40C9FF 10%, #E81CFF 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
