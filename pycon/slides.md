---
theme: seriph
background: >-
  https://github.com/LadyKerr/try-streamlit/assets/47188731/1af40df6-89a8-41bd-b7e0-dfa48682e652
title: How to get the  most out of your AI Pair Programmer
favicon: ''
font: Playfair Display
layout: cover
lineNumbers: true
transition: fade
record: dev
download: true
exportFilename: pycon-copilot
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

- What is GitHub Copilot?
- Tips to get the most out of GitHub Copilot
- Live Demo of GitHub Copilot with Jupyter NoteBooks, Python and ML 🐍
- Review
- Q&A & Resources

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
transition: fade-out
---

# What is GitHub Copilot?

### GitHub Copilot is an AI pair programmer that helps you write code faster.

<br>

![various-ide-copilot](https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/e39af215-9314-4524-8c23-eb3e0b280308)

![lprogramming-langauges](https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/94e3f958-bb51-4b47-b698-f6da3a992483)


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

<div class="absolute right-30px bottom-30px">
@itsthatladydev
</div>

<!--

But first, what is GitHub Copilot? :thinking:

Just in case you didn't know, GitHub Copilot is an AI pair programmer that helps you write code faster. It is designed to help with programming tasks and serves as your assistant while you're working in your IDE.

GitHub Copilot is comprised of a suite of products that goes beyond code completion.

Some of the tools that accompany GitHub Copilot includes a chat interface that you can use in your IDE, a command line tool via a GitHub CLI extension, GitHub Copilot for PRs, Copilot integrated into dotcom and many more. Today, we'll be looking at a few of the features that I've found to be most useful during my everyday development.

-->

---
transition: fade-out
layout: cover
background: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/9ac867c8-1ac1-45a7-b2e1-66f20bce4ad0
---

<!--

So, how many of you are using GitHub Copilot today?

So, how can we help GitHub Copilot help us?
The best thing we can do is to provide as much context as possible.

If you understand Large Language Models ( LLMs), you will know that they are designed to make predictions based on the context provided. This means, the more contextually rich our input or prompt is, the better the prediction or output will be.

Here are 6 tips to ensure that you're giving the best context to GitHub Copilot:

**1 - Open Files**
Copilot looks at the current and open files in your editor to analyze the context and create appropriate suggestions.

GitHub Copilot looks at the current open files in your editor to analyze the context, create a prompt that gets sent to the server, and return an appropriate suggestion.

Having your files open provides copilot with context. When you have additional files open, it will help to inform the completion that is returned. Remember if a file is closed, copilot cannot see that file's content. So have a few files open in your IDE to give GitHub Copilot a bigger picture of your project.


**2 - Provide a Top-level Comment**
Just as you would give a brief, high level intro to a coworker, a top level comment in the file you're working in can help Copilot understand the overall context of the pieces you will be creating.

This gives gh copilot a goal on what to work on. It helps to guide copilot to give better completions.


**3 - Appropriate Includes and references**
It's best to manually set the includes or module references you need for your work.

Copilot can make suggestions, but you likely know best what dependencies you'll need to include.

This can also help let Copilot know what frameworks, libraries, and their versions you'd like it to use when crafting suggestions.


**4 - Meaningful names matter!**
The name of your variables and functions matter. If you have a function named `foo` or `bar`, gh copilot will not be able to give you a good completion because it isn't able to infer intent from the name.

Just as the function name `fetchData()` won't mean much to a coworker (or you after a few months), `fetchData()` won't mean much to copilot either.

A lack of good coding practices will show up when you start using GitHub Copilot.


**5 - Specific and well scoped function comments**
Commenting your code helps you to get very specific targeted completions.

A function name can only be so descriptive without being overly long so function comments can help fill in details that Copilot might need to know.

Remember: Single, Specific, Short comments helps copilot provide better context.


**6 - Provide Sample Code**
Providing sample code to Copilot will help it determine what you're looking for. This helps to ground the model and provide it with more context.

It also helps gh copilot generate suggestions that match the language and tasks you want to achieve.

This can be especially helpful to jump start Copilot to a newer library version when it defaults to providing older code suggestions.


**Remember - Trust but verify!**
Do not trust the completion blindly. Always verify the completion before accepting it.

Top tip: The better the input, the better the output.

-->

---
layout: center
transition: fade-out
---
# DEMO TIME!

### repo: gh.io/pycon-demo

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

Demo notes

Building the API

So instead of using OPENAI api to get recommendations, 

<< open model file>>

I created a custom model that uses a perfume dataset from Kaggle to generate perfume recommendations for users.

I now want to take this model and build an API around it. I'll be using Flask to build the API.

<<open api file>>

You'll see I have a few imports already in the file and a simple hellp world route.

Let's ask Copilot to help us build out the recommendation route.

Ask: 

-->

---
transition: fade-out
---

# Resources


<div style="display: flex;">
  <div style="flex: 50%; padding: 10px;">
    <img src="https://github.com/LadyKerr/gh-copilot-talk/assets/47188731/cdea8189-2db9-4c51-9e67-281278312cf2" alt="using-copilot-tips" height="200" width="400">
  </div>
  <div style="flex: 50%; padding: 10px;">
    <img src="https://github.com/LadyKerr/gh-copilot-talk/assets/47188731/019dab54-13fe-4e79-8e13-a03dacf531e4" alt="using-copilot-tips" height="200" width="400">
  </div>
</div>

- **Demo repo** - gh.io/pycon-demo

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
layout: center
transition: fade-out
---
# Thank you!

> gh.io/pycon-demo

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