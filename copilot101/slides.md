---
theme: seriph
background: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/fbeeed3f-7a00-4b01-90a5-a4ea495a0f1c
title: Code Smarter not Harder with GitHub Copilot
favicon: ""
font: "Playfair Display"
layout: cover
lineNumbers: true
transition: fade
record: 'dev'
download: true
exportFilename: 'gh-copilot-101'
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
---

---
layout: image-right
image: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/7d0e2430-c5c9-483a-b8eb-afcda71e80f8
transition: fade-out
---

# Hi! I'm Kedasha!

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

Im super excited to talk to you about GitHub Copilot and how to get the most out of this tool. 

I know that AI has been the most used buzz word in the tech industry as of late and sometimes we may have the expectation that the AI tool we're implenting will do all the work for us. But just as we need to learn how to use a new framework or library, we also need to learn how to make AI tools work for us to get the results that we need. 

Today, I'll be sharing some pragmatic ways to get the most out of GitHub Copilot during your day to day development.
-->

---
layout: intro
transition: fade-out
---

# What we'll cover:

- What is GitHub Copilot?
- What is GitHub Copilot good for?
- BTS of GitHub Copilot Extension/Plugin
- Tips to get the most out of GitHub Copilot
- Live Demos
- Review
- Q&A

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
We'll take a brief look at what GitHub Copilot is, what it's good for, how it works, tips to get the most out of it, and then we'll do some live demos.
-->

---
transition: fade-out
---

# What is GitHub Copilot?

### GitHub Copilot is an AI pair programmer that helps you write code faster.

<br> 

<img src="https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/b3b0193f-913f-49b3-860e-9659db72a348" alt="GitHub Copilot" width="100%"/>

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

GitHub Copilot is comprised of a suite of products that goes beyond code completion.

Some of the tools that accompany GitHub Copilot includes a chat interface that you can use in your IDE, a command line tool via a GitHub CLI extension, GitHub Copilot for PRs, Copilot integrated into dotcom and many more. Today, we'll be looking at a few of the features that I've found to be most useful during my everyday development.

-->

---
transition: fade-out
---

# What is GitHub Copilot?

### You can use GitHub Copilot in your IDE. 
### It is available in VSCode, Neovim, Jetbrain IDE and Visual Studio.

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

<!--
To install it you'll go to your respective marketplaces for your IDE and install the extension. Once ut's installed you'll need to authenticate with your GitHub account. and if you have accesss, you'll be able to use GitHub Copilot in your IDE.

And it works with many languages - especially open source languages like javascript, typescript, python, java, python, go, ruby, and more.
-->

---
transition: fade-out
---

# What is GitHub Copilot good for?

- 🛠️ Boilerplate code and frameworks
- 🤷🏽‍♀️ Uncommon or confusing syntax
- 🔗 Pattern matching
- 👨🏽‍💻 Writing code faster
- ⛓️ Cron jobs and regex
- 👀 Helping you remember things you forgot
- 💻 Extending and refactoring existing code
- 🔖 Explaining unfamiliar code
- 📝 Documentation (which we all love to write!)
- 🚨 Understandiing error messages (and fixing it!)
- 🧪 Writing unit tests

. . . and much more! 🚀

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
Now what is GitHub Copilot good for?

Many things! Some of what it's best at is . . .
-->

---
transition: fade-out
---

# Some Limitations of GitHub Copilot 

- GitHub copilot != Compiler
- The AI cannot read your mind 
- The AI is not a replacement for good coding practices

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
It cannot read minds, although it sometimes feels like it can. It’s not a compiler, and it’s not a replacement for good coding practices. Actually if you have bad coding practices this will be more apparent when you use the AI because it uses the patterns in your code to give you suggestions.

This means, if you have bad coding practices, you’ll get bad suggestions. So it’s important to keep that in mind when you’re using it.

Also, one of the most important points I want to drive home today is that - GitHub Copilot is a tool that can help you write code faster, and it’s up to you to decide how to use it. 

It is not here to do your work for you or to write everything for you. It will guide you and nudge you in the right direction just as a coworker would if you asked them questions or for guidance on a particular issue.

-->

---
transition: fade-out
layout: image-left
image: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/c61055e8-7e8f-4b26-9f2a-a2074696863f 
---

# BTS of GitHub Copilot Extension/plugin

### GitHub Copilot draws context from the code you're working on to provide you with code suggestions.

<br>
<br>

## But what is included in this context? 🤔

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
transition: fade-out
layout: cover
background: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/02d1e0ce-8df1-483e-be84-4aa29235e4ef
---

<!--
Now let's zero in on the code completion feature of GitHub Copilot. 

When we look at the gh copilot ide extension, we see that it draws context from the code you're working on to provide you with code suggestions. 

As you're coding and as you add comments, GitHub Copilot will use that information to generate suggestions.

As you're typing your code and comments, context is sent up to GitHub Copilot. GitHub Copilot then uses the OpenAI LLM BTS, parses your requests and then returns a suggestion based on your request in your IDE. At this point, you can accept, reject or modify the provided suggestion.

This then means that you're able to provide as much context as possible to GitHub Copilot to get the best suggestions.

Today, I want to share with you 6 tips to get the most out of GitHub Copilot.

-->


---
transition: fade-out
layout: cover
background: https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/9ac867c8-1ac1-45a7-b2e1-66f20bce4ad0
---
<!--
So, how can we help GitHub Copilot help us?
The best thing we can do is to provide as much context as possible.

Here are 6 tips to ensure that you're giving the best context to GitHub Copilot:

**1 - Open Files**
Copilot looks at the current and open files in your editor to analyze the context and create appropriate suggestions.

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
transition: fade-out
layout: center
---

# D E M O S

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
transition: fade-out
---

<img src="https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/9ac867c8-1ac1-45a7-b2e1-66f20bce4ad0" alt="GitHub Copilot" width="100%"/>

---
transition: fade-out
layout: center
---

# Questions?

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
transition: fade-out
---

# Resources

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






