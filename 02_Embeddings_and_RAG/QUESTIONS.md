<p align = "center" draggable=”false” ><img src="https://github.com/AI-Maker-Space/LLM-Dev-101/assets/37101144/d1343317-fa2f-41e1-8af1-1dbb18399719" 
     width="200px"
     height="auto"/>
</p>

## <h1 align="center" id="heading">Session 2: Embeddings and RAG - Questions</h1>

#### ❓Question #1:

The default embedding dimension of `text-embedding-3-small` is 1536, as noted above. 

1. Is there any way to modify this dimension?
    ANSWER: reducing the dimensions parameter
2. What technique does OpenAI use to achieve this?
    ANSWER: the Matryoshka Representation Learning method

#### ❓Question #2:

What are the benefits of using an `async` approach to collecting our embeddings? ANSWER: concurrent processing can provide performance improvements 

#### ❓ Question #3:

When calling the OpenAI API - are there any ways we can achieve more reproducible outputs? ANSWER: keeping the temperature low to inhibit "creativity"

#### ❓ Question #4:

What prompting strategies could you use to make the LLM have a more thoughtful, detailed response? ANSWER: you could tell it to think step by step before providing a response, but reasoning models do not require this

What is that strategy called? ANSWER: chain of thought
