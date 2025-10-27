# Module 3: UX and Human in the loop
# Lesson 1: Streaming
1. Learned that LangGraph streaming gives us real-time updates as the graph runs. There are two main ways to see the state updates- first, updates which shows what changed only after a node ran. second, values which shows the full state after each node finishes.
2. I used the .astream_events method to stream tokens directly from the LLM and now know how to pull out the key parts of the event data: the event type, the name, the core data, and the metadata (which tells you which LangGraph node sent it).
3. I tweaked the code by adding self prompts as well as long message input.

# Lesson 2: Breakpoint
1. Learned that using breakpoints is how we implement Human in the Loop, stopping the graph until a person gives input. The main uses for HITL are approval, debugging and editing the state. I also learned to use graph.stream() to restart the graph from a saved checkpoint.
2. I tweaked by adding a breakpoint to pause the execution before the assistant node is called. I also defined and added several new tools to the list passed to the chat model, and updated the agent.py file to incorporate all these modifications.

# Lesson 3: Editing State and Human Feedback
1. Learned how to utilize breakpoints for more than just simple approval—they can now be used to directly modify the graph's state. This is a much more powerful form of Human-in-the-Loop (HITL) interaction. 
2. I tweaked the code by adding more tools to the existing tool list that is passed to the chat model. I also changed the prompts to test.
