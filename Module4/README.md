Module 4:

Lesson 1 - Parallelization
I learned how to build workflows in LangGraph that use parallel execution (fan-out) to run multiple steps at the same time. I saw how state reducers like operator.add are essential to safely merge the results from those concurrent nodes back into a single state key (fan-in).

Chnages made: I modified the RAG example by adding a new rephrase_question node that pre-processes the user's initial query before it's simultaneously sent to the search_web and search_wikipedia nodes.

<img width="1470" height="882" alt="Screenshot 2025-11-01 at 5 40 09 PM" src="https://github.com/user-attachments/assets/a7a1c4d1-f4cb-49d8-b2bb-3dc0e4612523" />

Lesson 2 - Sub-graphs
I learned how to define separate, independent graphs with their own state (sub-graphs) and then add them as nodes to a parent graph. This allows for building complex, multi-agent teams.

Changes made: I kept the parallel execution of the two sub-graphs, but I added a final `create_final_report` node that "fans-in" the outputs from both sub-graphs to create a single, combined summary.
