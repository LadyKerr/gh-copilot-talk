# Code Smarter not harder with GitHub Copilot - tips to get the most out of your AI pair programmer 🤖
> Demo repo: https://github.com/LadyKerr/mealmetrics-copilot/tree/demo on `demo` branch

## Outline:
- Intro
- What is GitHub Copilot?
- BTS of GitHub Copilot Extension/Plugin
- Gettiing the most out of GitHub Copilot
- Using GH Copilot to update a React component
- Using GH Copilot Chat to explain your code
- Using GH Copilot Chat to generate tests
- Using GitHub Copilot to write documentation
- Using Copilot to generate commit messages
- GitHub Copilot in the CLI (explain a cli command)
- GitHub Copilot in CLI (delete git branch locally and remotely)
- GitHub Copilot for PRs (create a new PR and generate a summary of work done)
- GitHub Copilot for PRs (highlight block of code in an open PR and ask to explain during review)
- GitHub Copilot on dotcom (slidev repo: ask how to create a new repo)
- Review: How to get the most out of copilot
- Review: Feats to make you a more productive developer

## Resources:

- Copilot tips from vscode team: https://twitter.com/code/status/1737903911237718467 
- VsCode docs on context: https://code.visualstudio.com/docs/editor/github-copilot 

## Intro

Hello! I'm Kedasha Kerr and Im a Developer Advocate at GitHub. Im super excited to talk to you about GitHub Copilot and how to get the most out of this tool. 

I know that AI has been the most used buzz word in the tech industry as of late and sometimes we may have the expectation that the AI tool we're implenting will do all the work for us. But just as we need to learn how to use a new framework or library, we also need to learn how to make AI tools work for us to get the results that we need. 

Today, I'll be sharing some pragmatic ways to get the most out of GitHub Copilot during your day to day development.

## What is GitHub Copilot?

But first, what is GitHub Copilot? :thinking:

Just in case you didn't know, GitHub Copilot is an AI pair programmer that helps you write code faster. It is designed to help with programming tasks and serves as your assistant while you're working in your IDE.

GitHub Copilot is comprised of a suite of products that goes beyond code completion.

Some of the tools that accompany GitHub Copilot includes a chat interface that you can use in your IDE, a command line tool via a GitHub CLI extension, GitHub Copilot for PRs, Copilot integrated into dotcom and many more. Today, we'll be looking at a few of the features that I've found to be most useful during my everyday development.

## What is GitHub Copilot Good for?

- Boilerplate code and frameworks 
- Uncommon or confusing syntax
- Pattern matching
- Writing code faster
- Cron jobs and regex
- Helping you remember things you forgot
- Extending and refactoring existing code
- Explaining unfamiliar code and documenting it
- Understandiing error messages (and fixing it!)
- Writing unit tests

. . . and more!

## Limitations of GitHub Copilot 🤔

- Training data impacts the quality of suggestions
- GitHub copilot != Compiler
- The AI cannot read your mind 
- The AI is not a replacement for good coding practices

## BTS of GitHub Copilot Extension/Plugin 👀

Now let's zero in on the code completion feature of GitHub Copilot. When we look at the gh copilot ide extension, we see that it draws context from the code you're working on to provide you with code suggestions. As you're coding and as you add comments, GitHub Copilot will use that information to generate suggestions.

As you're typing your code and comments, context is sent up to GitHub Copilot. GitHub Copilot then uses the OpenAI LLM BTS, parses your requests and then returns a suggestion based on your request in your IDE. At this point, you can accept, reject or modify the provided suggestion.

## More about Context

Now, let's talk more about the context because what exactly is being sent to GitHub Copilot? :thinking: 

**1 - the file you're currently working on**
The entire file, not just what is before and after the cursor. This is important because it allows GitHub Copilot to understand the context of the file you're working on.

**2 - tabs open in your IDE**
Tabs that are closest to the active tab are given priority assuming the're most closely related.

So just so we're on the same page, your entire reposirotry is not sent to GitHub Copilot. That would be a lot of information to send (read too many tokens) and would take a lot of time to process. Instead, GitHub Copilot uses the file you're working on and the tabs open in your IDE to generate suggestions.

Sending just these information allows copilot to focus on what is most important. We always want to keep the assistant focused on the task at hand.

## Getting the most out of GitHub Copilot 🛠️

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

## D E M O S 🎉

> Demo repo: https://github.com/LadyKerr/mealmetrics-copilot/tree/demo on `demo` branch
> recipe: 1 cup of all purpose flour, sifted 1 1/2 teaspoon baking powder 1/4 teaspoon salt 2 Tablespoon granulated sugar 1/2 Tablespoon unsalted butter, room temperature Approximately 1/3 cup water

### Demo 1: Split nutrition data in a new line so it's easier to read

Create a new file called `NutritionFacts.js`
Add a high level comment to the top of the file:

```
Create a component with the following specifications:

1. the component must split the received string data at /n/n or /n and return a Typography component for each string
2. the component must set a unique key for each Typography component
3. the component must return a div with the Typography components and return null if the data is not a string

```

> This address tips: high level comment, open files, includes & references

### Demo 2: Add a Footer Component

Create a new file called `Footer.js`

Add this comment first:

```
Add a footer component that says Made with love by LadyKerr & GitHub Copilot
```

After seeing the completion, reject it and add this comment:

```
Add a high level comment to the top of the file:
```
Create a footer component with the following specifications:

1. The footer must be fixed at the bottom of the page
2. Use the Paper and Typography components from Material UI
3. The footer text must say "Made with ❤️ by LadyKerr & GitHub Copilot"
4. The text "GitHub Copilot" must be a link to https://copilot.github.com/ that opens in a new tab with alt text "github copilot"
```

> This address tips: high level comment, open files, includes & references, meaningful names

### Demo 3: Add Documentation for a few functions

### Demo 4: Generate unit test for a function

### Demo 5: Check browser console for errors and have copilot explain it

### Demo 6: Click source control button and generate a commit message

### Demo 7: Copilot CLI explain a command and generate a command

### Demo 8: Copilot for PRs - generate a PR description

### Demo 9: Copilot on dotcom - ask questions about slidev repo

### Demo 10: Add theme for material UI to app (if time)





