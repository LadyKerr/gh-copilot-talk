# Langchain, OpenAI, LLMs, Oh My! Finding your way home through AI

## Talk Outline:
- What is an LLM?
- Key Terms and Definitions
- Brief History of LLMs
- How do LLMs work?
- Popular Language Models Today
- How do you choose the right LLM?
- How to use LLMs in your projects
- LangChain
- DEMO: Build a recommendation system with LLMs (rebuild noseNose rec system with LangChain)


## Resources:
- Attention is all you need: https://arxiv.org/abs/1706.03762 
- good article: https://thelowdown.momentum.asia/the-emergence-of-large-language-models-llms/
- excellent video: https://www.youtube.com/watch?v=osKyvYJ3PRM 
- great read by elastic: https://www.elastic.co/what-is/large-language-models 
- elastsearch langchain: https://www.elastic.co/search-labs/blog/large-language-models-elastic-code-langchain
- Demystifyig LLMs: https://github.blog/2023-10-27-demystifying-llms-how-they-can-do-things-they-werent-trained-to-do/ 
- AI for BEginners repo: https://github.com/microsoft/AI-For-Beginners 
- AL, ML, DL, GenAI: https://synoptek.com/insights/it-blogs/data-insights/ai-ml-dl-and-generative-ai-face-off-a-comparative-analysis/
- linkedin post: https://www.linkedin.com/posts/srikanth-reddy-98196712_ai-mldl-what-is-generative-ai-what-activity-7125167272247115777-Nobw/
- How LLMs work video: https://www.youtube.com/watch?v=5sLYAQS9sWQ 
- Gen AI in a nutshell: https://www.youtube.com/watch?v=2IK3DFHRFfw 
- How GitHUb Copilot handles data: https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/ 
- Top Open LLMs: https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard 
- The LLM Jourey: https://www.youtube.com/watch?v=jM72J9wPQQ0
- Story of Labguage Models: https://www.assemblyai.com/blog/the-full-story-of-large-language-models-and-rlhf/ 
- A Practical intro to LLMs (very good video!): https://www.youtube.com/watch?v=tFHeUSJAYbE
- build a LLM from scratch repo: https://github.com/rasbt/LLMs-from-scratch

The first AI tools had significant limitations - they couldnt understand context or learn and improve on their own.  the first chatbots for example were rule based, and relied on pre-defined rules or scripts with restricted user input. Thi srestricted their ability to understand and respond to user input. it only peformed th etasks it was programmed to do.

Intelligence as a Service 

## What is AI?

AI is the simulation of human intelligence processes by machines, especially computer systems. These processes include learning, reasoning, and problem solving.

AI is a broad field that includes many different types of technologies, such as machine learning, deep learning, and natural language processing.

## What is Machine Learning (ML)?

![Image](https://github.com/LadyKerr/ai-ml-notes/assets/47188731/4fde09d4-0093-46fc-8f49-46d2734e0a1f)

## What is Deep Learning (DL)?

## What is a neural network?

A neural network is a type of machine learning model that is inspired by the way the human brain works. It is a series of algorithms that tries to recognize patterns in data. 

The most important thing to keep in mind, is that neural networks simulate how the human brain works and large language models are a type of neural network that focuses on natural language.

[Intereact with a Neural Network online](https://github.com/tensorflow/playground)


# What is Natural Language Processing (NLP)?


## What is Generative AI?

Generative AI is a type of artificial intelligence that is capable of generating new content, such as images, text, or music. It is used in a variety of applications, such as chatbots, language translation, and text generation.

Some of the most common types of generative AI are:
- Generative Adversarial Networks (GANs)
- Variational Autoencoders (VAEs)
- Large Language Models (LLMs)

## What is an LLM?

LLMs are machine learning models capable of Natural Language Processing (NLP), as they are trained on huge amounts of text data (usually from the internet/books) via deep-learning algorithms. 

An LLM is a large language model, which is a type of neural network that is trained on large amoounts of text data. The model learns to generate text that is similar to the text it was trained on. LLMs are used in a variety of applications, such as chatbots, language translation, and text generation.

It is generally trained from data that can be found onlinie:
- books
- articles
- web scraping
- transcripts
- academic literature
- etc.

Anything that is text based can be traiined into an LLM. 

LLMs leverage transformer architectures to understand and generate coherent text based on given prompts. Transformer mdoels are the most common architecture of LLMs.

### Another definition

LLMs are generative AI models that generate text. They are trained on next token predictions and predict the next token based on the current token. They are looking for the most likely next token based on the tokens that came before it.

They have multilingual capabilities which means they've been trained on a multilingual context and they're very interactive. You can give them feedback if you dont like th eoutput and have a conversation with them to get where you want to go. 

### Problems LLM aims to solve:

- Enhancing communication
- Improving customer serveice
- education and learning
- content creation and analysis
- healthcare support
- data analysis 

### Architecture: Transformer Model (see image in google paper)

The transformer decoder is the core of the architecture of LLMs. It is designed to understand the context of a word in a sentence in relation to other words in the sentence. This is what makes transformers so powerful.





## Trad Programming vs LLMs
In traditional programming, it is very instructions based - if a then b - you're giving the computer a set of instructions to follow. With Large Language Models, you're teaching the computer how to learn how to do things providing a much more flexible and adaptable approach in programming. 

LLMs are used for a variety of tasks, such as:
- Chatbots
- Language translation
- Text generation
- Summarization
- Question answering
- Summarization
- Programming

## History and Evolution of LLMs
history of LLMS: https://toloka.ai/blog/history-of-llms/ 
ai timeline: https://voicebot.ai/large-language-models-history-timeline/ 

- 1924: The Ising Model, RNN [Recurrent Neural Network](https://arxiv.org/pdf/1801.01078) that did not learn
- 1943: Threshold Logic Unit (TLU), the first neural network
- 1966: ELIZA, the world's first chatbot and NLP model
- 1972: STNLP Statistically Trained Natural Language Processing System
- 1972: RNN, based on the ising model - able to learn. First technology that was able to predict the  next word in a sentence and not have everything pre-programmed for it. REVOLUTIONARY! Basis for how current LLMs work.
- 1997: LSTM, Long Short Term Memory, a type of RNN that can learn long term dependencies
- 1999: NVIDIA GPU - first Graphics Processing Unit, the GeForce 256
- 2000s: IBM Watson, a model that can answer questions
- 2010: CoreNLP from Stanford, a model that can parse and understand text
- 2011: Google Brain
- 2017: Transformers, Google transformer architecture (Attention is all your need, led OPENAI to develop chatGPT)
- 2013: Word2Vec, a model that can learn word embeddings
- 2018: GPT-1, the first large language model with 117m parameters
- 2018: BERT, Bidirectional Encoder Representations from Transformers, 340m parameters
- 2019: GPT-2, a larger version of GPT-1, 1.5b parameters
- 2020: GPT-3, the largest version of GPT, 175b parameters
- 2021: OpenAI Codex, natural language to code based on GPT-3
- 2021: GitHub Copilot Preview, a code completion tool based on Codex
- 2022: ChatGPT, a chatbot based on GPT-3
- 2022: GitHub Copilot GA, a code completion tool based on GPT-3
- 2024: GPT-4, the next version of GPT, 1.76 trillion parameters


## How do LLMs work?
NLP notes: https://github.com/LadyKerr/ai-ml-notes/blob/main/nlp.md 

To understand how LLMs work, let's take a look at how NLP works. NLP is used to standardize and analyze text data at scale. This includes:

- Cleaning and preprocessing text to reduce typos
- Remove unimportant words or phrases
- Parsing text into meaningful words or phases
- Converting text to numeric representations to perform statistical modeling easier
- Computing a degree of association between docs
- Getting structural and semantic meaning from text
- Organizing documents or efficient search

NLP has been in 
- languge translation
- ranking newsfeed on social media 
- highligting relevant reviews on e-commerce sites

The NLP process follows the following pipeline:
- Tokenization: breaking down text into smaller units (words, phrases, etc.)
- Preprocessing: cleaning and normalizing text (removing punctuation, lowercasing, removing stop words, etc.)
- Featutrization: converting text into numerical representations (word embeddings, TF-IDF, vectorization, etc.)
- Modeling: training a model to predict or classify text data (classification, regression, clustering, etc.)


## How LLMs work:  

- Data
millions and millions of data points are used to train LLMs. The more data you have, the better your model will be.


- Architectre: Transformer architecture allows the model to understand sequences of data. Transformers are the most common architecture of LLMs. They are designed to understand the context of a word in a sentence in relation to other words in the sentence.

-  Training
The model is then trained on all the data gathered to predict the next word in a sentence. The model is trained to predict the next word in a sentence based on the words that came before it. The model is trained to generate text that is similar to the text it was trained on.


LLMs can be finetuned to perform specific tasks. For example, you could take a pre-trained language model and fine-tune it on a dataset of movie reviews to make it better at generating movie reviews. Fine-tuning is a powerful technique that can help you get better results with less data and less training time.

Fine tuning allows a general language model to become an expert in a specific domain or task.

## Transformers

GPT: Generative Pre-trained Transformer

Generative: generate new text
Pre-trained: process of learning from a large dataset
Transformer: a neural network (ml model) that is designed to understand sequences of data. It is core to the architecture of LLMs and current boom in AI.

Because of transformers, we can product an image froom text, produce audio from text, create videos from text, and even generate code from text.

Transformers were invented in 2017 by Google for a specific task: translate text from one language into another. They were able to translate text from one language to another with a high degree of accuracy. They were able to do this by understanding the context of a word in a sentence in relation to other words in the sentence. This is what makes transformers so powerful.


When we give a text to a language model, the text is broken up into tiny pieces called tokens. Each token is then converted into a numerical representation (vector) that the model can understand. The model then uses these numerical representations to generate text that is similar to the text it was trained on.


## LLMs Training Process

With LLMs specifically, the training looks like:
- Data Collection
- Tokenization
- Model Training
- Testing

The first step of training a large language model is to collect a large dataset of text data. This dataset can be collected from a variety of sources, such as books, articles, web scraping, transcripts, academic literature, etc. The more data you have, the better your model will be. However, you need to make sure that your data is clean and free of errors, as this can negatively impact the performance of your model. Having a good dataset that is representative of the text data you want to generate is key to training a successful large language model. Garbage in = garbage out.

You must have good clean data to train your LLMs. You need a LOT of data - BILLIONS and BILLIONS of parameters. You need to have a good dataset to train you models. If you have terrible data going in your will have terrible data coming out. If a dataset is biased, your model will be biased. If a dataset contains racism, your model will be racist. So it is important to have a good dataset to train your model.

We all want to avoid having badly built models.
Datasets are HUGE. I dont think we can comprehend how big these datasets are.

"LLMs are not trained to reason. They’re not trying to understand science, literature, code, or anything else. They’re simply trained to predict the next token in the text." - Alireza Goudarzi, Senior ML Researcher, GitHub Copilot

 ## Tokens visualized

- 260 tokens look like this:
- 100,000 tokens look like this:
- 1,000,000 tokens look like this:
- 1 billion tokens look like this:


Trainings models is extremely expensive and time consuming. It can take weeks to train a model. 

## Fine Tuning

Fine tuning is the process of taking a pre-trained model and training it on a smaller dataset to adapt it to a specific task. This is useful when you have a pre-trained model that is already good at generating text, but you want to make it better at a specific task. 

For example, you could take a pre-trained language model and fine-tune it on a dataset of movie reviews to make it better at generating movie reviews. Fine-tuning is a powerful technique that can help you get better results with less data and less training time.

## Limitations of LLM

- struggle a lot with math and reasoning 
- BIAS. LLMs don't reflect the real world. 40% of the world doesnt have internet access. Data trained the ai is generated by humans, so therefore it will contain bias.
- Knowledge is up until their traing occur. This is changing with RAG, browsing internat, access to realtime data. 
- Hallucinations - the model can generate text that is confidently incorrect.
- Cost a lot of money to train and to fine tune
- Ethical considerations: copyright material used to train, privacy, etc.
- Models being used for harmful purposes: deep fakes, misinformation, scams, etc.
- Considerations: AGI. What happens when we reach AGI? Will we be able to control it? Will it be able to control us? Will it be able to control itself? 

## real World Applications of LLMs

- Language Transation
- Coding
- Summarization
- Content Creation
- image to animation: https://www.tiktok.com/@teaonadawnsha/video/7375172934131879214?is_from_webapp=1&sender_device=pc&web_id=7272496714942416426 (tiktok example that uses jst-1 model that understands physics and can animate an image to an example video: https://viggle.ai/; closed source model)
- Image generation (text to image): ![chat-gpt-bleach-blonde](https://github.com/LadyKerr/llms-oh-my/assets/47188731/2e423252-7d14-4c1a-a881-3815424e9fe7)


## Model Types

- text to text 
- text to code
- text to image
- text to audio
- text to video
- text to animation
- text to 3D model


## Popular Language Models Today (add params to models)

- Google Gemma
- Anthropic Claude 
- OpenAI GPT-4
- Meta Llama3
- Mistral AI Mistral
- Microsoft phi3
- TogetherAI

## How to choose the right LLM?

- What is your use case?
- What is your budget?
- What is your timeline?
- What is your data?
- What is your team's expertise?
- What is your model's performance?
- What is your model's interpretability?
- What is your model's scalability?
- What is your model's ethical considerations?

## How to use LLMs in your projects

- Choose the right model
- Collect and clean your data
- Train your model
- Fine-tune your model
- Test your model
- Deploy your model
- Monitor your model
- Update your model

## LangChain

Langchain is a developer-friendly toolkit that simplifies the process of creating applications powered by large language models (LLMs). It provides tools, abstractions, and integrations to make it easier to work with these models.

Langchain essentially acts as a bridge between your application and the power of large language models, making it easier to incorporate sophisticated AI features into your projects.

-------------------------
-------------------------


** A C T U A L  T A L K  N O T E S 📚 ** 

## Outline:

- What is an LLM?
    - AI -> ML -> DL -> NLP -> Generative AI -> LLM
    - Define and explain Large Language Models (LLMs)
    - Popular Language Models Today
- Step back: Brief History of LLMs
- How do LLMs work? How were they built?
    - Data Collection
    - Transformer Architecture
    - Training Process 
    - Tokenization
    - Optimization 
    - Evaluation
- Key Terms and Definitions
        - Tokens
        - Transformers
        - Attention Mechanism
        - Pre-training 
        - Fine Tuning
        - Embeddings
        - Context Window
        - Language Model Benchmarking (GLUE and SuperGLUE)
- How do you choose the right LLM? https://youtu.be/tFHeUSJAYbE?si=dawN6BaPYxoh_92x&t=505 
    - Prompt Engineering
    - Fine Tuning
    - Build Your Own
- Building with LLMS:
    - LLM use cases
    - use each model's api
    - use a tool like LangChain
- LangChain 
- DEMO
- Resources to learn more
- Q&A

