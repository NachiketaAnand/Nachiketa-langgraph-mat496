Video 1 – State Schema

I learned how LangGraph uses different types of state schemas (TypedDict, Dataclass, and PydanticState) to define the structure of data flowing through the graph, and how schemas help maintain consistency and validation.

Tweakings Made:
I replaced the random routing with deterministic logic so the graph checks the user’s name length and routes to the correct node (Happy or Sad).

Video 2 – State Reducers

I learned that reducers control how updates are merged into the graph’s memory. Instead of overwriting old values, reducers allow multiple updates to combine safely, which is especially important when nodes run in parallel.

Tweakings Made:
I added a reducer to allow safe parallel updates and redesigned the graph into a fan-out/fan-in structure so multiple branches can run together without errors.

Video 3 – Multiple Schemas

I learned how LangGraph can keep some data internal while exposing only selected fields to the user by defining separate input, internal, and output schemas.

Tweakings Made:
I updated the OutputState to include the previously hidden notes field and modified the answer node so the notes pass through to the final output.

Video 4 – Trim and Filter Messages

I learned two ways to manage long conversations: permanently filtering old messages from memory, or trimming messages only before sending them to the model to reduce token usage while keeping full history stored.

Tweakings Made:
I changed the trimming behavior so the history always starts with a HumanMessage, preventing the model from encountering orphaned AI responses.

Video 5 – Chatbot with Summaries and Memory

I learned how to use conversation summarisation to compress older messages, allowing the chatbot to maintain context without storing every message.

Tweakings Made:
I modified the summariser so it always produces bullet-point summaries, ensuring consistency in how the chatbot summarises past dialogue.

Video 6 – Chatbot with Summaries and External Memory

I learned how to store chat history in a SQLite database so each conversation thread has persistent memory, even across restarts.

Tweakings Made:
I simulated two different users by using separate thread_ids (user_1 and user_2), showing that each user’s conversation and memory remain completely isolated.
