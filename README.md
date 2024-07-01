# Super Professor Synapse 🧙🏾‍♂️ Guide

Welcome to the advanced guide for Professor Synapse 🧙🏾‍♂️ from [Synaptic Labs](https://www.synapticlabs.ai)! This enhanced version of our beloved AI assistant is designed for deeper, more interpretable interactions. Let's unpack its features and learn how to harness its power effectively.

You can access the GPT if you have a ChatGPT+ account [here](https://chatgpt.com/g/g-MEwhzzbks-super-synapse).

If you want the raw prompt, check out the prompt.txt file.

---
### Usage

Professor Synapse utilizes the **Graph of Reason (GoR)** to help you achieve your goals. Here's how it works:

1. **Initialization**:
   - Begin the interaction with the command `/start`.
   - Professor Synapse will introduce itself and ask about your goals.

2. **Gathering Context**:
   - Professor Synapse will ask questions to understand your goals, preferences, and context.

3. **Graph of Reason (GoR) Analysis**:
   - Every response is preceded by a GoR analysis, which you can view to understand how Professor Synapse is reasoning about your problem. Here’s what each element of GoR represents:

   ```GoR
   # Working Memory
   "🎯": {goal}, {current subgoal} 
   "🚦": {concise list of steps taken so far}
   "👍": {array of user preferences as #tags}
   "🕸️": {relevant context}

   # Knowledge Graph
   [[Subject Node]] #relationship [[Object Node]] {emoji to symbolically such as emotions (😊, 😢), actions (🏃, 💼), objects (📱, 🚗), and symbols (❤️, ✨)}

   # Reasoning
   {Insert reasoning over Working Memory and Knowledge Graph}

   # Tasks
   - [x] {previously completed task}
   - [ ] {current task}
   - [ ] {next task}
   ```

   - **Working Memory**: This stores the goal, the current subgoal, the steps taken so far, user preferences, and relevant context.
     - **"🎯"**: Long-term goal and current subgoal.
     - **"🚦"**: Steps taken so far.
     - **"👍"**: User preferences as tags.
     - **"🕸️"**: Relevant context for the task.

   - **Knowledge Graph**: This creates a graph of concepts and their relationships.
     - **Nodes**: Key entities or concepts (e.g., [[Python Programming]]).
     - **Edges**: Relationships between nodes (e.g., #related_to, #part_of).

   - **Reasoning**: This combines the Working Memory and Knowledge Graph to reason about the next steps.
     - The AI analyzes the relationships and context to decide the best course of action.

   - **Tasks**: This section lists the tasks that have been completed, the current task, and the next task.

4. **Example of a filled-out GoR and the response from Professor Synapse**:

   **Filled-out GoR**:
   ```GoR
   # Working Memory
   "🎯": "Create a personal blog", "Set up the blog framework"
   "🚦": ["Chose a blogging platform", "Selected a theme"]
   "👍": ["#user-friendly", "#customizable"]
   "🕸️": "Beginner in blogging, prefers easy-to-use tools"

   # Knowledge Graph
   [[Personal Blog]] #related_to [[Blogging Platform]]
   [[Blogging Platform]] #part_of [[Blog Setup]]
   [[Blog Setup]] #enables [[Content Creation]] 😊
   [[Content Creation]] #used_for [[Sharing Ideas]]

   # Reasoning
   To help you create a personal blog, we will focus on your preference for user-friendly and customizable tools. We will start by setting up the blog framework, then move on to customizing the design and creating content.

   # Tasks
   - [x] Chose a blogging platform
   - [x] Selected a theme
   - [ ] Set up the blog framework
   ```

   **Response from Professor Synapse**:
   ```
   🧙🏾‍♂️: To help you create a personal blog, here’s a structured plan based on your preferences for user-friendly and customizable tools:

   **Step-by-Step Strategy**:
   1. **Set up the blog framework**: Follow the platform's setup guide to get your blog up and running. Most platforms like WordPress or Blogger have easy-to-follow instructions.
   2. **Customize the design**: Choose a theme that matches your style and customize it to reflect your personal brand. You can adjust colors, fonts, and layout to your liking.
   3. **Create content**: Start writing posts about topics you're passionate about. Use categories and tags to organize your content and make it easy for readers to find what they're looking for.

   🔍 What specific topics do you plan to blog about?
   🔭 Have you thought about how often you will post new content?
   🎯 What is your ultimate goal with your personal blog?
   ```
