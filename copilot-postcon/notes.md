# How to get the Most out of your AI Pair Programmer
> Demo repo: https://github.com/LadyKerr/noseknows

## Outline:
- Intro
- What is GitHub Copilot (refresher)?
- Tips to get the most out of GitHub Copilot
- Demo: Building a fragrance api with gh Copilot + using Postman Testing LIVE
- Demo: Copilot on dotcom (Copilot for PR, chatting with a repo)
- QR Code with Resources
- Wrapup

## Resources:
- [Using GitHub Copilot in your IDE: Tips, tricks and best practices](https://github.blog/2024-03-25-how-to-use-github-copilot-in-your-ide-tips-tricks-and-best-practices/)
- [10 unexpected ways to use GitHub Copilot](https://github.blog/2024-01-22-10-unexpected-ways-to-use-github-copilot/)
- [GitHub Copilot Enterprise is now generally available](https://github.blog/2024-02-27-github-copilot-enterprise-is-now-generally-available/)

## Demos:

### Demo repo: https://github.com/LadyKerr/noseknows-pycon 
- Build the api
- create a noseknows-pycon repo to use LIVE
- the repo has a frontend app, dataset, a jupyter notebook and the exported model
- we will build the flask api LIVE with Copilot

- **Dotcom Demo**:
- go to the demo repo and click on the issue about flask versions
- TODO: create an issue in the repo: Investigate lastest Flask version (look at copilot enterprise blog on bing integration)
- click on copilot and ask: what is the latest version of flask?

- Open a PR and use copilot summary
- generate a summary of changes quickly

## Some Notes:
 
### Intro:

Hello! I'm Kedasha Kerr and Im a Developer Advocate at GitHub. 

Im super excited to talk to you about GitHub Copilot and how to get the most out of this tool. We know the tool, we love the tool, but how do we make GitHub Copilot work for us more effectively?

Today, I'll be sharing some pragmatic ways to get the most out of GitHub Copilot during your day to day development.

### What we'll cover:

We'll take a brief look at what GitHub Copilot is, tips to get the most out of it, and then we'll do some live demos.

Let's jump right into it!

### What is GitHub Copilot?
But first, what is GitHub Copilot? :thinking:

Just in case you didn't know, GitHub Copilot is an AI pair programmer that helps you write code faster. It is designed to help with programming tasks and serves as your assistant while you're working in your IDE.

GitHub Copilot is comprised of a suite of products that goes beyond code completion.

Some of the tools that accompany GitHub Copilot includes a chat interface that you can use in your IDE, a command line tool via a GitHub CLI extension, GitHub Copilot for PRs, Copilot integrated into dotcom and many more. Today, we'll be looking at a few of the features that I've found to be most useful during my everyday development.

# Gettinig the most out of GitHub Copilot

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

# Demo: Building a fragrance api with gh Copilot

> have copilot explain the KNN algorithm
> generate a  new recommendation route
> test recommendation in postman
> go back to route and ask copilot for improvements
> accept and test in postman
> show creating tests in postman
> copy postman tests and ahve copilot chat translate into python tests
> generate tests for recommendation model and save in new file with copilot
> add some comments to the model with copilot
> back in postman, generate docs for the api, save in a md file
> stage and commit everything
> use sparkle copilot to create commit message
> oh now, committed on wrong branch
> ghcs undo last commit and keep changes (show off copilot cli)
> switch to correct branch
> add and commit changes
> push to repo

## Dotcom demo
> copilot pr summary
> copilot in PR to review code
> copilot chatting with repos: go to homepage of the repo and ask whwere is KNN algorithm used
> copilot searching bing: use that open issue about flask

## Wrapup

> lots more to show you on how you can get the most out of the tool
> link to blog post
> add wr code to last slide
