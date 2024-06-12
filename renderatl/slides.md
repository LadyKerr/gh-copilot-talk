---
theme: seriph
title: Beyond the Editor - tips to get the most out of GitHub Copilot
background: https://cover.sli.dev
favicon: ''
font: Playfair Display
layout: cover
lineNumbers: true
transition: fade
record: dev
download: true
exportFilename: renderatl-slides
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
---

<!--
Hello good morning! Thank you all for being here with me today to learn all about large Language Models.

-->

---
layout: image-right
image:  https://github.com/LadyKerr/mealmetrics-copilot/assets/47188731/7d0e2430-c5c9-483a-b8eb-afcda71e80f8
transition: fade-out
---

# Hi! I'm Kedasha!

- Jamaican gyal! 🇯🇲 
- Developer Advocate at GitHub 
- Software Developer for ~4 years 
- Technical Content Creator ✨ 
- Newly minted AI/ML enthusiast 🤖

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
introduce self
-->


---
layout: intro
transition: fade-out
---

# What we'll cover:

- What is an LLM?
- How do LLMs Work?
- Key Terms to know
- Building with LLMs?
- The Langchain effect
- Live Demo
- Resources to learn more
- Q&A 


<!--

Here's a quick overview of what we'll be covering today - attempt to cover today in the next 40mins or so.

-->

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
layout: image
image: https://github.com/LadyKerr/llms-oh-my/assets/47188731/43116e62-af4e-49c6-b70e-e98fcb667a23
transition: fade-out
---

<!--

Sooo, earlier this year I embarked on a journey to learn more about AI and ML and gain some foundational knowledge in the field. I then started to learn about and build with large language models (and even built my own custom model) and I'm here to share some of that knowledge with you today.

-->

---
layout: image-left
image: https://github.com/LadyKerr/llms-oh-my/assets/47188731/0980bf0c-ed23-4f61-b978-74ff6ade15db
transition: fade-out
---

# Large Language Models

- Have you used one before? 🤔

- Do you know how they work? 🤯

![Image](https://github.com/LadyKerr/llms-oh-my/assets/47188731/2f7df360-a359-4ff5-be27-aca41495d1d1)


<!--

Now, how many of you have used an LLM before? Im expecting to see a lot of hands here because of ChatGPT
And how many of you actually understand what an LLMs and how they work?

-->

---
layout: image-right 
image:  https://github.com/LadyKerr/llms-oh-my/assets/47188731/c8bede3f-2b8f-4a36-88f8-57466eb25919
transition: fade-out
---

# What is an LLM?

## Large - > 1 billion parameters (referes to LARGE corpus of data)
## Language -> Text generation and understanding
## Model -> A system that learns from data

<!--

A large langage model is a type of generative AI that can generate human-like text. These models are trained on vast amounts of text data and are able to generate text that is coherent and contextually relevant.

But, when we talk about AI and their relationship with LLMs, we must look at the sort of hierachal relationship that exists between the two.

AI can be considered as Mother - the parent of Machine Learning, Deep Learnig, Natural Language Processing, Generative AI and Large Language Models.

AI is the research and implementation of systems that are able to pperform tasks intelligently.

ML is where computers learn from data in order to make predictions. A key thing to remember about ML is that a model is the core output and the goal is to be able to make accurate predictions on new previously unseen data.

When we get to the deep learning portion of things, this is where neural networks are used to solve complex problems. A neural network is essentially where the human brain is mimicked in a computer system. This allows computers to recognize patterns that is able to solve complex problems like image recognition, speech recognition and natural language processing (NLP).

Once we get to the NLP of things, this is where we are able to teach computers to understand and generate human language. Now Natural Language Processing  is a branch of AI that enables computers to understand language in the form of text and spoken words. And "natural language" refers to the way humans communicate with each other in their native tongue - english, spanish, french, portuguese etc. are all examples of natural languages.

NLP has many use cases such as:
- document summarization
- language translation
- automatic virtual agents and chatbots
- classifying social  media comments as positive or negative

and so on. 

Ok sooo NLP leads us to Generative AI. Generative AI is a type of artificial intelligence that is capable of generating new content, such as images, text, or music.

Some of the most common types of generative AI are:
- Generative Adversarial Networks (GANs)
- Variational Autoencoders (VAEs)
- Large Language Models (LLMs)

We'll be focusing on Large Language Models today.

BUT you can see the relationship between AI and LLMs right? AI is Mother and LLMs are the children of AI. And thanks to the multi year advanmcements in AI, we now have LLMs that are being integrated into our daily lives in ways we never thought possible or only dreameed of.

Some people dont think that LLMs are AI but when you look at these layers and how they relate to each other you can really see that without AI, LLMs would not exist.

-->


---
layout: intro
transition: fade-out
---

# Popular Language Models today 

- Google Gemma
- Anthropic Claude 
- OpenAI GPT-4
- Meta Llama3
- Mistral AI Mistral
- Microsoft phi3
- TogetherAI

<!--

Some of the most popular LLMs today include . . .
 . .  and these are all forms of generative AI. 
To get to the point of having al these LLMs, we must first understand the building blocks of these models - transformers.

Let's take a step back in history for a second.
-->


---
layout: intro
transition: fade-out
---

# Brief History of LLMs

1925 - The Ising Model - the 1st RNN that did not learn
1966 - ELIZA - the world's first chatbot and NLP model
1972 - RNNs (Recurrent Neural Networks)
1997 - LSTM (Long Short Term Memory) - a type of RNN that can learn long term dependencies
2017 - Transformer Models
2018 - GPT-1, the first large language model introduced by OPENAI, 117 million parameters
2018 - BERT (Bidirectional Encoder Representations from Transformers), 340 million parameters
2019 - GPT-2, 1.5 billion parameters
2020 - GPT-3, 175 billion parameters
2021: OpenAI Codex, natural language to code based on GPT-3
2021: GitHub Copilot Preview, a code completion tool based on Codex
2022: ChatGPT, a chatbot based on GPT-3
2024: GPT-4, the next version of GPT, 1.76 trillion parameters


<!--

In the 60's ELIZA was created by an MIT researcher and was able to hold a conversation with a human user by following a pre-written script.
This was revolutionary at the time and many felt like they were talking to a real person.

Flash forward a few years and we had RNNs and LSTMs. RNNs were actually able to learn. They were the first technology that was able to predict the  next word in a sentence and not have everything pre-programmed for it. REVOLUTIONARY! Basis for how current LLMs work and they're actually a part of popular tech today like Siri, Alexa and Google Translate.

Long Short Term Memory were able to learn from data and generate text and started to revolutionize speech recognition and machine translation in the early 2000s.

Then, in 2017, Google introduced Transformer models. These models were neural networks that were able to learn context, and find relationships between words in a sentence. This was a game changer in the world of NLP and the foundation for the LLMs we have today.

They are also called Foundation Models and they use attention or self attention to figure out the subtleties of language. This was revolutionary and everytime we search on Google, we are using a transformer model.

Then in 2018, we got Generative Pre-trained Transformer 1 (GPT-1), the first large language model introduced by OPENAI that utilized Google's Transformer model. It had 117 million parameters which is like.

Once transformers and GPT-1 came to the scene, things started to move pretty rapidly. In 2018, BERT was introduced by Google. Then in 2019, we got GPT-2, from OPEN-AI, then GPT-3 in 2020. GPT-3 had 175 billion parameters and was the largest LLM at the time.

Then in 2021, we got Codex, a natural language to code model based on GPT-3. And then GitHub Copilot Preview, a code completion tool based on Codex. And then in 2022, we got ChatGPT, a chatbot based on GPT-3.

And that changed EVERYTHING.

ChatGPT was the first LLM that was able to hold a conversation with a human user and it was able to generate human-like text that was coherent and contextually relevant. IT WAS AMAZING!! Do you remember the first time you used chatGPT?? I do! It was like magic!

And so, Transformers truly changed everything and is the basis for how LLMs work today. Let's take a deeper look at how LLMs actually work and how they were built.
-->


---
layout: intro
transition: fade-out
---

# How do LLMs Work? How were they built?

Transformers are the building blocks of LLMs ✨

- Data Collection
- Transformer Architecture
- Training Process 
- Tokenization
- Optimization 
- Evaluation


<!--

-->

---
layout: intro
transition: fade-out
---

## Key Terms to know
- Tokens
- Transformers
- Attention Mechanism
- Pre-training 
- Fine Tuning
- Embeddings
- Context Window
- Language Model Benchmarking (GLUE and SuperGLUE)


<!--

-->

---
layout: intro
transition: fade-out
---


insert text needed here

<!--

-->

---
layout: intro
transition: fade-out
---

# How do you choose the right LLM?



<!--

-->

---
layout: intro
transition: fade-out
---


# The Langchain effect


<!--
Langchain is a framework that was developed to make it easier for any developer to build their own LLM powered application. It currently suports 2 languages - Python and Javascript.


-->

---
layout: intro
transition: fade-out
---

# Live Demo


<!--

-->

---
layout: intro
transition: fade-out
---

# Q&A and Resources


<!--

-->