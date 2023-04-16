# Azure-OpenAI

There has been a massive buzz these days around the Large Language Models (LLM), especially now that everyone can access the GPT models via ChatGPT and try out its wonderful capabilities. For developers like us, who have been working in the domain of natural language processing for some years, language models are not new. This time, I got an opportunity to participate in a hackathon using Azure OpenAI APIs to solve business use-cases.

I came across several wonderful blogs/reading materials on how to use LLMs for production. I learnt about prompt engineering and how to use prompts effectively to gradually achieve the desired outcome. This blog is a great introduction to prompts: https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/guides/prompts-intro.md

Some basic tips recommended to design prompts are:
1. Keep the value of the temperature parameter low to avoid randomness and obtain more determninistic results (depends on the application, for creative applications we can keep this value high).
2. Using simple and specific instructions return better results.
3. It is better to mention what to do, instead of defining what not to do. 

Prompt Engineering are ways to modify the prompts without updating the model weights, so as to steer the model's response. 

Methods like Zero-Shot Learning and Few-Shot learning are some of the basic approaches that can be used to interact with the model. In Zero Shot learning, we simply ask the model what we want from it. In Few Shot learning, we show the model some good examples of the input and the kind of output that we expect from the model. This is expected to return better results than Zero Shot approach. 

I also realised that:
1. While natural language interface is much convenient for users, it isn't the cause of a great developer experience. This is because a slight change in the prompt can return very different output which is difficult to detect.
2. We can mitigate the ambiguity in LLM's response, by systematically applying prompt engineering. 

This repository contains some of my experimentation with using Azure OpenAI APIs and prompt engineering.