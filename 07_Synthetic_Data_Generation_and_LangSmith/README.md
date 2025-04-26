
<p align = "center" draggable=”false” ><img src="https://github.com/AI-Maker-Space/LLM-Dev-101/assets/37101144/d1343317-fa2f-41e1-8af1-1dbb18399719" 
     width="200px"
     height="auto"/>
</p>

## <h1 align="center" id="heading">Session 7: Synthetic Data Generation and LangSmith</h1>

| 🤓 Pre-work | 📰 Session Sheet | ⏺️ Recording     | 🖼️ Slides        | 👨‍💻 Repo         | 📝 Homework      | 📁 Feedback       |
|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|
| [Session 7: Pre-Work](https://www.notion.so/Session-7-Synthetic-Data-Generation-for-Evaluation-1c8cd547af3d81999da6cbd18ae4b6a9?pvs=4#1c8cd547af3d81edb0f8ca8017d1cfdb)| [Session 7: Synthetic Data Generation for Evaluation](https://www.notion.so/Session-7-Synthetic-Data-Generation-for-Evaluation-1c8cd547af3d81999da6cbd18ae4b6a9) | [Recording](https://us02web.zoom.us/rec/share/fSb3DEXkbvGFQgQwwXY9Htm7CzLKXqTuOscraGRRFaj7bC7XIODwhgP2VgXpx1Uu.dKkuAcnlOrlQ7Bcq) (M9g55ye#) | [Session 7: Synthetic Data Generation for Evaluation](https://www.canva.com/design/DAGjaZbyELk/2hj3-ZHrH6x4kjz1Y3kAYw/edit?utm_content=DAGjaZbyELk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)| You Are Here!| [Session 7: Synthetic Data Generation for Evaluation](https://forms.gle/DVmFHjkkgFpAKNoEA)| [AIE6 Feedback 4/22](https://forms.gle/Z1DahTCVsNPp6SrU6)

In today's assignment, we'll be creating Synthetic Data, and using it to benchmark (and improve) a LCEL RAG Chain.

- 🤝 BREAKOUT ROOM #1
  1. Use RAGAS to Generate Synthetic Data

- 🤝 BREAKOUT ROOM #2
  1. Load them into a LangSmith Dataset
  2. Evaluate our RAG chain against the synthetic test data
  3. Make changes to our pipeline
  4. Evaluate the modified pipeline

## Ship 🚢

The completed notebook!

#### 🏗️ BONUS ACTIVITY (OPTIONAL):

Reproduce the RAGAS Synthetic Data Generation Steps - but utilize a LangGraph Agent Graph, instead of the Knowledge Graph approach.

This generation should leverage the [Evol Instruct](https://arxiv.org/pdf/2304.12244) method to generate synthetic data.

Your final state (output) should contain (at least, not limited to):

1. `List(dict)`: Evolved Questions, their IDs, and their Evolution Type.
2. `List(dict)`: Question IDs, and Answer to the referenced Evolved Question.
3. `List(dict)`: Question IDs, and the relevant Context(s) to the Evolved Question.

The Graph should handle:

1. Simple Evolution.
2. Multi-Context Evolution.
3. Reasoning Evolution.

It should take, as input, a list of LangChain Documents.

### Deliverables

- A short Loom of the notebook, and a 1min. walkthrough of the application in full

## Share 🚀

Make a social media post about your final application!

### Deliverables

- Make a post on any social media platform about what you built!

Here's a template to get you started:

```
🚀 Exciting News! 🚀

I am thrilled to announce that I have just built and shipped Synthetic Data Generation, benchmarking, and iteration with RAGAS & LangChain! 🎉🤖

🔍 Three Key Takeaways:
1️⃣ 
2️⃣ 
3️⃣ 

Let's continue pushing the boundaries of what's possible in the world of AI and question-answering. Here's to many more innovations! 🚀
Shout out to @AIMakerspace !

#LangChain #QuestionAnswering #RetrievalAugmented #Innovation #AI #TechMilestone

Feel free to reach out if you're curious or would like to collaborate on similar projects! 🤝🔥
```



#### ❓ Question #1:

What are the three types of query synthesizers doing? Describe each one in simple terms.

I found a reference here: https://docs.ragas.io/en/stable/concepts/test_data_generation/rag/

A single-hop query is a question that requires retrieving information from a single document or source to provide a relevant answer. It involves only one step to arrive at the answer.  ** In this example 50% of the queries are single-hop.

A multi-hop query involves multiple steps of reasoning, requiring information from two or more sources. The system must retrieve information from various documents and connect the dots to generate an accurate answer.

- the abstract query requires the retrieval of multiple pieces of information over time and across different sources to form a broad, interpretive response.  ** In this example 25% of the queries are multi-hop abstract.

- the specific query focuses on clear, fact-based retrieval.  ** In this example 25% of the queries are multi-hop specific.

#### 🏗️ Activity #2:

Highlight what each evaluator is evaluating.

- `qa_evaluator`: question answer evaluator evaluates the accuracy of the model answers compared to the reference answers, did it correctly anser the question
- `labeled_helpfulness_evaluator`: evaluates the response by using the llm response and the reference answer to determine helpfulness, how helpful the response may be to the user
	* compare the strings for answers and determine if the submission was helpful
	* prediction output = is what chain gives us
	* reference is our answer = reference answer created by ragas
	* input the question
- `dope_or_nope_evaluator`: evaluates the response to determine how dope, lit or cool the llm response is


#### ❓Question #2:

Why would modifying our chunk size modify the performance of our application?

smaller chunks would perform faster and prob use less tokens, but maybe lose some meaning

semantic chunking is much more accurate but potentially less performant than smaller chunking strategies like word or sentence


#### ❓Question #3:

Why would modifying our embedding model modify the performance of our application?

each embedding model has it's own performance characteristics, quality and speed can vary based on the model.  some are better suited to specific tasks, ie sentiment.

#### 🏗️ Activity #3:

Provide a screenshot of the difference between the two chains, and explain why you believe certain metrics changed in certain ways.

Screenshot 2025-04-26 155939.png