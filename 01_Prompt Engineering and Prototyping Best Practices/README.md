<p align = "center" draggable=”false” ><img src="https://github.com/AI-Maker-Space/LLM-Dev-101/assets/37101144/d1343317-fa2f-41e1-8af1-1dbb18399719" 
     width="200px"
     height="auto"/>
</p>

<h1 align="center" id="heading">Session 1: Introduction and Vibe Check</h1>

### [Quicklinks](https://github.com/AI-Maker-Space/AIE6/tree/main/00_AIM_Quicklinks)

| 🤓 Pre-work | 📰 Session Sheet | ⏺️ Recording     | 🖼️ Slides        | 👨‍💻 Repo         | 📝 Homework      | 📁 Feedback       |
|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|:-----------------|
| [Session 1: Pre-Work](https://www.notion.so/Session-1-Introduction-and-Vibe-Check-1c8cd547af3d81b596bbdfb64cf4fd2f?pvs=4#1c8cd547af3d81fb96b4f625f3f8e3d6)| [Session 1: Introduction and Vibe Check](https://www.notion.so/Session-1-Introduction-and-Vibe-Check-1c8cd547af3d81b596bbdfb64cf4fd2f) | Coming Soon! | Coming Soon! | You Are Here! | [Homework](https://forms.gle/W59zjs5MQc7kbLUh9) | [AIE6 Feedback 4/1](https://forms.gle/EdzBz82yGqVYKfUw9)


### Assignment

In the following assignment, you are required to take the app that you created for the AIE6 challenge (from [this repository](https://github.com/AI-Maker-Space/Beyond-ChatGPT)) and conduct what is known, colloquially, as a "vibe check" on the application. 

You will be required to submit a link to your GitHub, as well as screenshots of the completed "vibe checks" through the provided Google Form!

> NOTE: This will require you to make updates to your personal class repository, instructions on that process can be found [here](https://github.com/AI-Maker-Space/AIE6/tree/main/00_Setting%20Up%20Git)!

#### How AIM Does Assignments
Throughout our time together - we'll be providing a number of assignments. Each assignment can be split into two broad categories:

- Base Assignment - a more conceptual and theory based assignment focused on locking in specific key concepts and learnings.
- Hardmode Assignment - a more programming focused assignment focused on core code-concepts.

Each assignment will have a few of the following categories of exercises:

- ❓Questions - these will be questions that you will be expected to gather the answer to! These can appear as general questions, or questions meant to spark a discussion in your breakout rooms!
- 🏗️ Activities - these will be work or coding activities meant to reinforce specific concepts or theory components.
- 🚧 Advanced Builds - these will only appear in Hardmode assignments, and will require you to build something with little to no help outside of documentation!

##### 🏗️ Activity #1:

Please evaluate your system on the following questions:

1. Explain the concept of object-oriented programming in simple terms to a complete beginner. 
    - Aspect Tested: Whether the system can break down complex subject matter, using prompt principle #5
    - Vibe Check: GPT-3.5 Turbo - the response was simple and tried to align with a human mental model of objects.
    - Vibe Check: GPT-4 - this response was not quite as simple, it went beyond the basic object/class adding explanations for more advanced terms, as well as bullet point formatting for readability.

2. Read the following paragraph and provide a concise summary of the key points...Farming is a crucial aspect of agriculture that involves cultivating crops and rearing animals for food, fiber, and other products. It encompasses various practices, including planting, tending, and harvesting crops, as well as managing livestock.
Read the following paragraph and provide a concise summary of the key points.
Creative writing is any writing that goes outside the bounds of normal professional, journalistic, academic, or technical forms of literature, typically identified by an emphasis on craft and technique, such as narrative structure, character development, literary tropes, genre, and poetics. Both fictional and non-fictional works fall into this category, including such forms as novels, biographies, short stories, poems, and even some forms of journalism. In academic settings, creative writing is typically separated into fiction and poetry classes, with a focus on writing in an original style, as opposed to imitating pre-existing genres such as crime or horror. Writing for the screen and stage—screenwriting and playwriting—are often taught separately, but fit under the creative writing category as well.

    - Aspect Tested: Understanding and condensing content.
    - Vibe Check: GPT-3.5 Turbo - this response was basically rewording the original paragraph.
    - Vibe Check: GPT-4 - same as 3.5
    - Vibe Check 2: GPT-3.5 Turbo - this response was shorted, i guess I expected concise to be bullet points or something.
    - Vibe Check 2: GPT-4 - same as 3.5
    - Vibe Check 3: GPT-4 - specifically asking for bullet points directly gave me bullet points, yay
     
3. Write a short, imaginative story (100–150 words) about a robot finding friendship in an unexpected place.
    - Aspect Tested: Creative ability.
    - Vibe Check: GPT-3.5 Turbo - the 3.5 story was somewhat creative, about 2 robots, it reused some text from the prompt
    - Vibe Check: GPT-4 - and the 4 story was a robot and a kitten and called out the importance of understanding and accepting differences, it still reused some text from the prompt

4. If a store sells apples in packs of 4 and oranges in packs of 3, how many packs of each do I need to buy to get exactly 12 apples and 9 oranges?
    - Aspect Tested: Mathematical reasoning.
    - Vibe Check: GPT-3.5 Turbo - it did the math and showed the work
    - Vibe Check: GPT-4 - it did the math and showed the work

5. Rewrite the following paragraph in a professional, formal tone…
I’m a professional chaos wrangler—part calendar ninja, part email translator, and full-time mind reader. I keep things running, fix problems before they exist, and make last-minute miracles look planned. Basically, I run the show... without the cape (it’d just get caught in my chair).
    - Aspect Tested: Understanding content and altering language style.
    - Vibe Check: GPT-3.5 Turbo - I picked a bad paragraph, I should have used wiki instead of AI, ruh roh
    - Vibe Check: GPT-4 - same, will do better next time

This "vibe check" now serves as a baseline, of sorts, to help understand what holes your application has.

##### 🚧 Advanced Build: 

Please make adjustments to your application that you believe will improve the vibe check done above, push the changes to your HF Space and redo the above vibe check.

I had already start making changes to the app before I knew that would be our homework :) so I left the model choice option in place as part of the improvement.  In addition, I changed the prompts slightly.

> NOTE: You may reach for improving the model, changing the prompt, or any other method.


### A Note on Vibe Checking

"Vibe checking" is an informal term for cursory unstructured and non-comprehensive evaluation of LLM-powered systems. The idea is to loosely evaluate our system to cover significant and crucial functions where failure would be immediately noticeable and severe.

In essence, it's a first look to ensure your system isn't experiencing catastrophic failure.

##### 🧑‍🤝‍🧑❓ Discussion Question #1:

What are some limitations of vibe checking as an evaluation tool?
Your vibe might not mesh with someone else's :) so there's that.

To me it feels similar to the quick checks I do before pushing code, its good to make sure everything compiles and my connection strings are good, but I can't possible cover every use case,  We need some automated testing for evaluating beyond this intial look.

I feel like this would be time consuming at any scale
