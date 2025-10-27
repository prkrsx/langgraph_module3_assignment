# Module 3: UX and Human in the loop
# Lesson 1: Streaming
1. Learned that LangGraph streaming gives us real-time updates as the graph runs. There are two main ways to see the state updates- first, updates which shows what changed only after a node ran. second, values which shows the full state after each node finishes.
2. I used the .astream_events method to stream tokens directly from the LLM and now know how to pull out the key parts of the event data: the event type, the name, the core data, and the metadata (which tells you which LangGraph node sent it).
3. I tweaked the code by adding self prompts as well as long message input.

